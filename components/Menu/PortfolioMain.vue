<template>
  <div>
    <div class="container py-40">
      <div class="flex text-start ">
        <h1 class="font-bold text-white text-[50px]">PORTFOLIO</h1>
      </div>


      <div class="gallery-wrap">
        <ul id="filters" class="clearfix ">
          <li @click="filterGallery('all')">
            <span :class="{ active: activeFilter === 'all' }" class="filter"><i data-v-56c03d90="" data-v-ff212fc2="" class="icon hover:text-red-500 text-[#979798] group-hover:text-[#00A795] duration-300"><svg width="22" height="33" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" clip-rule="evenodd" d="M18.8571 0H15.7143C13.9786 0 12.5714 1.40721 12.5714 3.14286V6.28571C12.5714 8.02136 13.9786 9.42857 15.7143 9.42857H18.8571C20.5928 9.42857 22 8.02136 22 6.28571V3.14286C22 1.40721 20.5928 0 18.8571 0ZM18.8571 12.5714H15.7143C13.9786 12.5714 12.5714 13.9786 12.5714 15.7143V18.8571C12.5714 20.5928 13.9786 22 15.7143 22H18.8571C20.5928 22 22 20.5928 22 18.8571V15.7143C22 13.9786 20.5928 12.5714 18.8571 12.5714ZM6.28571 12.5714H3.14286C1.40721 12.5714 0 13.9786 0 15.7143V18.8571C0 20.5928 1.40721 22 3.14286 22H6.28571C8.02136 22 9.42857 20.5928 9.42857 18.8571V15.7143C9.42857 13.9786 8.02136 12.5714 6.28571 12.5714ZM6.28571 0H3.14286C1.40721 0 0 1.40721 0 3.14286V6.28571C0 8.02136 1.40721 9.42857 3.14286 9.42857H6.28571C8.02136 9.42857 9.42857 8.02136 9.42857 6.28571V3.14286C9.42857 1.40721 8.02136 0 6.28571 0Z" fill="#979798"></path>
</svg>
</i></span>
          </li>
          <li @click="filterGallery('print')">
            <span :class="{ active: activeFilter === 'print' }" class="filter">Branding</span>
          </li>
          <li @click="filterGallery('strategy')">
            <span :class="{ active: activeFilter === 'strategy' }" class="filter">Mobile app</span>
          </li>
          <li @click="filterGallery('logo')">
            <span :class="{ active: activeFilter === 'logo' }" class="filter">CRM</span>
          </li>
          <li @click="filterGallery('web')">
            <span :class="{ active: activeFilter === 'web' }" class="filter">Website</span>
          </li>
        </ul>

        <div id="gallery" data-aos="fade-up">
          <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-10 items-center">
            <div
                v-for="item in filteredItems"
                :key="item.id"
                :class="['gallery-item', item.category]"
                :data-cat="item.category"
                data-aos="fade-right"
            >
              <NuxtLink :to="`/products/${item.id}`">
                <div class="inside">
                  <div class="details">
                    <div class="text bg-emerald-950 rounded-[50%] p-2">
                      <i><img src="../../assets/images/arrow-right-line-uic.png" class="" alt="no arrow"></i>
                    </div>
                  </div>
                  <div class="overlay"></div>
                  <img :src="item.image" class="w-full h-[280px] rounded-[12px] overflow-hidden" alt="no image" />
                </div>
              </NuxtLink>

            </div>
          </div>

        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import {ref, computed, onMounted} from 'vue';
import AOS from 'aos';
import 'aos/dist/aos.css'

const activeFilter = ref('all');
const galleryItems = ref([
  {
    id: 1,
    client: 'https://remixicon.com/icon/arrow-right-line',
    type: 'Logo',
    category: 'print',
    image: 'https://uic.group/media/cache/0c/39/0c392b9a99ead3fb208087f2a1e1e145.jpg',
  },
  {
    id: 2,
    client: 'Client Name',
    type: 'Logo',
    category: 'Web',
    image: 'https://uic.group/media/cache/29/88/29883e26588ac429b3ca86b3ac39efa6.jpg',
  },
  {
    id: 3,
    client: 'Client Name',
    type: 'Web',
    category: 'web',
    image: 'https://uic.group/media/cache/cc/39/cc392cc7e6083d974df22bdf3f7baae3.jpg',
  },
  {
    id: 4,
    client: 'Client Name',
    type: 'Print',
    category: 'print',
    image: 'https://uic.group/media/cache/59/f1/59f1ca58bab7263f9c5eaff3033d5951.jpg',
  },
  {
    id: 5,
    client: 'Client Name',
    type: 'Strategy',
    category: 'strategy',
    image: 'https://uic.group/media/cache/b6/27/b6273a3cbd3fe1e5ad0e9b9acdccdfc4.jpg',
  },
  {
    id: 6,
    client: 'Client Name',
    type: 'Strategy. Web. Print.',
    category: 'strategy web print',
    image: 'https://uic.group/media/cache/77/4d/774ddc33fda844b44bb597539531dec6.jpg',
  },
  {
    id: 7,
    client: 'Client Name',
    type: 'Web',
    category: 'web',
    image: 'https://uic.group/media/cache/b3/6b/b36bc02390ec157e4a4a99eb5c0643b2.jpg',
  },
  {
    id: 8,
    client: 'Client Name',
    type: 'Strategy',
    category: 'strategy',
    image: 'https://uic.group/media/cache/cc/39/cc392cc7e6083d974df22bdf3f7baae3.jpg',
  },
  {
    id: 9,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/30/da/30da918dacc113dd034fb5dbb8063282.jpg',
  },
  {
    id: 10,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/d4/e7/d4e7073d362f8d5a16efbb3e656fc4ee.jpg',
  },
  {
    id: 11,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/30/da/30da918dacc113dd034fb5dbb8063282.jpg',
  },
  {
    id: 12,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/a8/77/a87702a9481ecefa9ba4b96e95167d43.jpg',
  },
  {
    id: 13,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/f3/0c/f30c607df76522d92e14712217621ac9.jpg',
  },
  {
    id: 14,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/06/93/06932db52dc70fee360b1432daafa68c.jpg',
  },
  {
    id: 15,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/a9/6e/a96ed6470476a8cacc4cde4a1d3a8ef6.jpg',
  },
  {
    id: 16,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/40/18/40184a46e212d8e0e613fc4c5536ca3a.jpg',
  },
  {
    id: 17,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/d1/96/d1961f8f4931839e7a777b05da15fdf3.jpg',
  },
  {
    id: 18,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/43/20/4320381fb20cd336dc90868ff2bfe386.jpg',
  },
  {
    id: 19,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/2a/14/2a146e3dd5a0701fb3eacc6c3373eb4d.jpg',
  },
  {
    id: 20,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/57/e0/57e0493ebac4d57a20ef41b751c4848a.jpg',
  },
  {
    id: 21,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/aa/06/aa061770c62851026e6a8594e375dcc5.jpg',
  },
  {
    id: 22,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/b8/92/b89267f245fbbd0ab6acebc63fb72d21.jpg',
  },
  {
    id: 23,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/6a/78/6a78330ad1b1291390e179bbdb074851.jpg',
  },
  {
    id: 24,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/61/8d/618dca95e4ab8ec44157ecce89185989.jpg',
  },
  {
    id: 25,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/3f/75/3f7537cdf56c38afa9367478f052e265.jpg',
  },
  {
    id: 26,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/fa/4f/fa4f66e1e9ad3e87f35badec0259d415.jpg',
  },
  {
    id: 27,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/ef/5a/ef5a4b196a41591e8b5f650dc36699c0.jpg',
  },
  {
    id: 28,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/2a/ab/2aabe99d837aa97e6aa3edbb3342c104.jpg',
  },
  {
    id: 29,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/74/72/7472f7a10311c94fa1794af99a6f454e.jpg',
  },
  {
    id: 30,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/d8/a4/d8a4a3b10b14a9224a0337b7472b30ec.jpg',
  },
  {
    id: 31,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/c0/49/c0493bad7ba2684dbc8265bcfe3858d7.jpg',
  },
  {
    id: 32,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/12/4d/124d9a091b727f4149fdc7fc25cbf47c.jpg',
  },
  {
    id: 33,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/67/c0/67c022e8e5b7c730fe4d5ef0fac8fbc1.jpg',
  },
  {
    id: 34,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/be/00/be0021e030433a9fa7d98d35ea0daf12.jpg',
  },
  {
    id: 35,
    client: 'Client Name',
    type: 'Strategy. Web.',
    category: 'web strategy',
    image: 'https://uic.group/media/cache/b7/a6/b7a6bd7a6eb6e10b337dbccfa5c8e7af.jpg',
  },
]);

onMounted(() => {
  AOS.init ({
    duration: 1000,
    easing: 'ease-in-out',
    once: true,
  })
})


const filterGallery = (category) => {
  activeFilter.value = category;
};

const filteredItems = computed(() => {
  if (activeFilter.value === 'all') {
    return galleryItems.value;
  }
  return galleryItems.value.filter(item => item.category.includes(activeFilter.value));
});
</script>

<style scoped lang="scss">
@import 'https://fonts.googleapis.com/css?family=Lato|Roboto+Slab:700';

html {
  box-sizing: border-box;
}









.container {
  margin: 0 auto;
  max-width: 1300px;
  width: 100%;
}

h1 {
  text-align: center;
  margin: 50px 0;
}

.gallery-wrap,
#gallery {
  overflow: hidden;
}

#filters {
  margin: 1%;
  padding: 0;
  list-style: none;
  overflow: hidden;
  margin-bottom: 60px;
}

#filters li {
  float: left;
}

#filters li span {
  display: block;
  margin: 10px;
  border-radius: 12px;
  padding: 10px 30px;
  text-decoration: none;
  border: 2px solid #666;
  color: #666;
  font-size: 20px;
  font-weight: 600;
  cursor: pointer;
  transition: 0.5s ease;
}

#filters li:hover span {
  color: #666;
}

#filters li span.active {
  background: transparent;
  border: 2px solid #1a8377;
  border-radius: 12px;
  color:#fff;
}

.gallery-item {

}

.inside {
  position: relative;
  overflow: hidden;
  width: 100%;
  height: 100%;
}

.details,
.overlay {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  opacity: 0;
  border-radius: 12px;
}

.details {
  display: flex;
  align-items: end;
  justify-content: end;
  padding: 15px;
  z-index: 2;
  transition: all 0.3s ease-in-out;
  i {
    color: #fff;
    font-size: 1.5em;
    font-weight: 700;
    letter-spacing: 1px;
    text-align: center;
    margin: 0;
  }
}

.inside img {
  float: left;
  width: 100%;
  filter: brightness(60%);
}

.overlay {
  background:
      linear-gradient(160deg, rgba(45, 184, 147, 0.64), rgba(45, 184, 147, 0.25), rgba(67, 67, 67, 0.10), rgba(45, 184, 147, 0.54),);
  z-index: 1;
  transition: all 0.7s ease-in-out;
}

.gallery-item:hover .details,
.gallery-item:hover .overlay {
  opacity: 1;
}

@media (max-width: 30em) {
  .wrap {
    padding-left: 1em;
    padding-right: 1em;
  }

  .gallery-item {
    float: none;
    width: 100%;
  }
}

@media(max-width: 656px){
  #filters{
    display: grid;
    grid-template-columns: repeat(2, 1fr);
  }
}
</style>
