<template>
  <div>
    <div class="container mt-40">


      <div class="content">
          <div
              v-for="(image, index) in paginatedItems"
              :key="index"
              class="image-container"
          >
              <section class="h-full-0" data-aos="fade-up">
                <div class="grid grid-cols-2 gap-[5rem] bg-[#222222] cursor-pointer group-hover:" data-aos="zoom-in-right">
                  <!-- Blog post -->

                  <article class="">
                    <a class="relative block group" href="#">
                      <div class="absolute inset-0 bg-[#333333] md:block transform md:translate-y-44 md:translate-x-44 xl:translate-y-4 xl:translate-x-8 group-hover:translate-x-0 group-hover:translate-y-0 transition duration-700 ease-out pointer-events-none" ></div>
                      <figure class="relative h-0 pb-[86.25%] md:pb-[105%] lg:pb-[76.25%] overflow-hidden transform md:-translate-y-2 xl:-translate-y-4 group-hover:translate-x-0 group-hover:translate-y-0 transition duration-700 ease-out">
                        <img class="absolute inset-0 w-full h-full z-50 transform hover:scale-105 transition duration-700 ease-out" :src="image"  alt="Blog post">
                      </figure>
                    </a>
                    <div>
                      <header>
                        <div class="mb-3">
                          <!--                      <ul class="flex flex-wrap text-xs font-medium -m-1">-->
                          <!--                        <li class="m-1">-->
                          <!--                          <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-purple-600 hover:bg-purple-700 transition duration-150 ease-in-out" href="#0">Product</a>-->
                          <!--                        </li>-->
                          <!--                        <li class="m-1">-->
                          <!--                          <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-blue-500 hover:bg-blue-600 transition duration-150 ease-in-out" href="#0">Engineering</a>-->
                          <!--                        </li>-->
                          <!--                      </ul>-->
                        </div>
                        <!--                    <h3 class="text-2xl lg:text-3xl font-bold leading-tight mb-2">-->
                        <!--                      <a class="hover:text-gray-100 transition duration-150 ease-in-out" href="#0">Designing a functional workflow at home.</a>-->
                        <!--                    </h3>-->
                      </header>

                    </div>
                  </article>

                  <div v-for="item in uic" :key="item.title"
                  >
                    <div class="flex flex-col gap-10 items-center">
                      <h1 class="mt-10 text-white">{{item.title}}</h1>
                      <p class="text-xl">{{item.description}}</p>

                      <div class="flex gap-20 items-start  justify-start p-4">
                        <hr class="text-white opacity-30">
                        <div class="flex gap-4 items-center">
                          <i data-v-56c03d90="" class="icon hover:text-red-500"><svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M1.86133 5.50245H12.1444" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                            <path d="M9.5629 7.75558H9.56824" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                            <path d="M7.00284 7.75558H7.00818" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                            <path d="M4.4379 7.75558H4.44324" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                            <path d="M9.5629 9.99781H9.56824" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                            <path d="M7.00284 9.99781H7.00818" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                            <path d="M4.4379 9.99781H4.44324" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                            <path d="M9.33315 1.23076V3.12929" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                            <path d="M4.67299 1.23076V3.12929" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                            <path fill-rule="evenodd" clip-rule="evenodd" d="M9.44557 2.14183H4.56058C2.86634 2.14183 1.80811 3.08564 1.80811 4.8205V10.0414C1.80811 11.8036 2.86634 12.7692 4.56058 12.7692H9.44022C11.1398 12.7692 12.1927 11.82 12.1927 10.0851V4.8205C12.198 3.08564 11.1452 2.14183 9.44557 2.14183Z" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                          </svg>
                          </i>

                          <p>10.12.2022</p>
                        </div>

                        <div class="flex gap-4 items-center">
                          <i data-v-56c03d90="" class="icon hover:text-red-500"><svg width="14" height="14" viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M0.583496 6.99996C0.583496 6.99996 2.91683 2.3333 7.00016 2.3333C11.0835 2.3333 13.4168 6.99996 13.4168 6.99996C13.4168 6.99996 11.0835 11.6666 7.00016 11.6666C2.91683 11.6666 0.583496 6.99996 0.583496 6.99996Z" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                            <path d="M7 8.75C7.9665 8.75 8.75 7.9665 8.75 7C8.75 6.0335 7.9665 5.25 7 5.25C6.0335 5.25 5.25 6.0335 5.25 7C5.25 7.9665 6.0335 8.75 7 8.75Z" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                          </svg>
                          </i>
                          <p>1240</p>
                        </div>

                      </div>

                    </div>

                  </div>
                </div>
              </section>
            <!--          <img :src="image" loading="lazy" alt="image item" />-->
          </div>
      </div>

      <div class="pagination">
        <div @click="goToFirst">&#171</div>
        <div @click="prevPage">&lt</div>
        <div class="numbers">
          <div
              v-for="page in visiblePages"
              :key="page"
              :class="{ current: currentPage === page }"
              @click="goToPage(page)"
          >
            {{ page }}
          </div>
<!--          <div v-for="index in uic" :key="index"-->
<!--          >-->
<!--            <h1>{{index.title}}</h1>-->
<!--          </div>-->
        </div>
        <div @click="nextPage">&gt</div>
        <div @click="goToLast">&#187</div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, computed, onMounted } from 'vue';
import AOS from 'aos';
import 'aos/dist/aos.css';

// Fetch images from API
const getImages = async (maxImages = 1) => {
  const url = `https://picsum.photos/v2/list?limit=${maxImages}`;
  const response = await fetch(url);
  const data = await response.json();
  return data.map(image => image.download_url);
};

// Reactive state
const totalItems = ref(100);
const perPage = ref(12);
const currentPage = ref(1);
const imagesList = ref([]);
const totalPages = computed(() => Math.ceil(totalItems.value / perPage.value));
const maxVisibleButtons = ref(5);

// Computed properties for pagination
const paginatedItems = computed(() => {
  const start = (currentPage.value - 1) * perPage.value;
  return imagesList.value.slice(start, start + perPage.value);
});

const visiblePages = computed(() => {
  const maxLeft = Math.max(1, currentPage.value - Math.floor(maxVisibleButtons.value / 2));
  const maxRight = Math.min(totalPages.value, currentPage.value + Math.floor(maxVisibleButtons.value / 2));

  let pages = [];
  for (let page = maxLeft; page <= maxRight; page++) {
    pages.push(page);
  }
  return pages;
});

// Pagination controls
const nextPage = () => {
  if (currentPage.value < totalPages.value) {
    currentPage.value++;
  }
};

const prevPage = () => {
  if (currentPage.value > 1) {
    currentPage.value--;
  }
};

const goToPage = (page) => {
  currentPage.value = page;
};

const goToFirst = () => {
  currentPage.value = 1;
};

const goToLast = () => {
  currentPage.value = totalPages.value;
};

// Fetch images and initialize
onMounted(async () => {
  imagesList.value = await getImages(totalItems.value);
});

onMounted(() => {
  AOS.init({
    duration: 1000, // Duration of the animation
    easing: 'ease-in-out', // Easing function
    once: true, // Whether animation should happen only once
  });
});

const uic = [
  {
    id: 1,
    title: "Opportunity for an internship at the UIC Group in the direction of Project Manager",
    description: "The team of the UIC Group welcomes everyone on the day of the adoption of the Constitution of the Republic of Uzbekistan, December 8th.",
  },
]
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Sansita+Swashed:wght@400;500&display=swap');

$mainColor: #2c3e50;
$secondaryColor: #3498db;



.container {
max-width: 1320px;

  h2 {
    color: #eee;
  }

  .content {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    align-items: center;
    justify-content: center;
    gap: 5rem;

    .image-container {

      img {
        width: 650px;
        height: 100%;
        box-shadow: 2px 2px 5px 0 rgba(0, 0, 0, 0.3);
        object-fit: cover;
        //filter: blur(4px);
        overflow: hidden;
        transition: 0.2s linear;

        &:hover {
          cursor: pointer;
          transform: scale(1.05);
          filter: blur(0);
          box-shadow: 5px 5px 15px 0 rgba(0, 0, 0, 0.5);
        }
      }
    }
  }

  .pagination {
    display: flex;
    align-items: center;
    justify-content: end;
    gap: 2rem;
    font-size: 15px;
    padding: 15px;
    color: #eee;

    div:not(.numbers) {
      cursor: pointer;
      padding: 8px;

      &:hover {
        color: #1a8377;
      }
    }

    .numbers {
      display: flex;
      align-items: end;
      justify-content: end;
      gap: 2rem;

      .current {
        display: flex;
        align-items: center;
        color: white;
        border: 2px solid #1a8377;
        border-radius: 12px;
        padding: 8px 17px 8px 17px;

        &:hover{
        }
      }
    }
  }
}
</style>
