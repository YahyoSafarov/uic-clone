React Vue Nuxt TypeScript Js, [6/8/2024 11:01 AM]
<template>
  <div>
    <div class="section-padding gallery-section" id="gallery">
      <div class="container">
        <!-- Section Title Start -->
        <div class="text-center">
          <h2 class="title">Our Gallery</h2>
          <p>Some Random Photos Lorem ipsum, dolor sit.</p>
        </div>
        <!-- Section Title End -->

        <div id="btncontainer" class="filter">
          <button :class="{ 'btn-active': activeFilter === 'all' }" class="btn" @click="filterGallery('all')">ALL</button>
          <button :class="{ 'btn-active': activeFilter === 'Bollywood' }" class="btn" @click="filterGallery('Bollywood')">Bollywood</button>
          <button :class="{ 'btn-active': activeFilter === 'Hollywood' }" class="btn" @click="filterGallery('Hollywood')">Hollywood</button>
          <button :class="{ 'btn-active': activeFilter === 'tv' }" class="btn" @click="filterGallery('tv')">TV Shows</button>
        </div>

        <!-- Gallery Section Start -->
        <div class="gallery sets">
          <a v-for="(img, index) in filteredImages" :key="index" @click="openImage(index)">
            <img :src="img.src" />
          </a>
        </div>
      </div>
    </div>

    <div v-if="isModalOpen" class="openDiv">
      <img :src="images[currentImage].src" class="imgPreview" />
      <div class="butonsSection">
        <button class="prevButton" @click="prevImage">Previous</button>
        <button class="nextButton" @click="nextImage">Next</button>
      </div>
      <button class="closeBtn" @click="closeModal">Close</button>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const activeFilter = ref('all');
const currentImage = ref(0);
const isModalOpen = ref(false);

const images = ref([
  { src: 'https://iili.io/y7W4t4.md.webp', category: 'Bollywood' },
  { src: 'https://i.redd.it/a90376enwvg91.jpg', category: 'Bollywood' },
  { src: 'https://iili.io/y7waOg.md.jpg', category: 'Bollywood' },
  { src: 'https://iili.io/y7WrNf.webp', category: 'Bollywood' },
  { src: 'https://i.redd.it/wh6hbexev2v91.jpg', category: 'Hollywood' },
  { src: 'https://i.redd.it/4b6s83hss9p91.jpg', category: 'Hollywood' },
  { src: 'https://i.redd.it/2s7w09k01ol91.jpg', category: 'tv' },
  { src: 'https://i.redd.it/2s7w09k01ol91.jpg', category: 'tv' },
]);

const filteredImages = computed(() => {
  if (activeFilter.value === 'all') return images.value;
  return images.value.filter(img => img.category === activeFilter.value);
});

const filterGallery = (filter) => {
  activeFilter.value = filter;
};

const openImage = (index) => {
  currentImage.value = index;
  isModalOpen.value = true;
};

const closeModal = () => {
  isModalOpen.value = false;
};

const nextImage = () => {
  currentImage.value = (currentImage.value + 1) % images.value.length;
};

const prevImage = () => {
  currentImage.value = (currentImage.value - 1 + images.value.length) % images.value.length;
};
</script>

<style scoped>
a {
  text-decoration: none;
  cursor: pointer;
  outline: 0;
}

.section-padding {
  padding-top: 80px;
}

.gallery-section {
  position: relative;
  z-index: 1;
}

.title {
  font-size: 46px;
  font-weight: 700;
  font-family: 'Playfair Display', serif;
  color: #f44336;
}

.filter {
  text-align: center;
  max-width: 1050px;
  margin: auto;
}

.btn {
  padding: 10px 20px;
  margin: 5px 4px 4px 0;
  display: inline-block;
  color: #003;
  background: #eee;
  border: 1px solid #f44336;
  transition: all 0.4s;
  border-radius: 10px;
  font-size: 16px;
  font-weight: 500;
}
.btn:hover, .btn-active {
  background: #f44336;
  color: #fff;
  transform: translateY(3px);
}

.gallery {
  display: flex;
  justify-content: center;
  width: fit-content;
  max-width: 1320px;
  flex-wrap: wrap;
  margin: 25px auto;
}
.gallery a {
  display: flex;
}
.gallery img {
  width: 200px;
  height: 220px;
  object-fit: cover;
  transition: 0.3s ease-in-out;
  border-radius: 12px;
  overflow: hidden;
  margin: 10px 10px;
}

.gallery img:hover {
  transform: scale(1.1);
}

.sets .hide,
.sets .pophide {
  width: 0%;
  opacity: 0;
}

React Vue Nuxt TypeScript Js, [6/8/2024 11:01 AM]
.closeBtn {
  position: absolute;
  font-size: 22px;
  font-weight: 500;
  right: 25px;
  top: 25px;
  color: white;
  transition: 0.5s linear;
  padding: 8px 40px;
  border-radius: 25px;
  background: red;
  outline-offset: -6px;
  outline: 2px solid #fff;
}
.closeBtn:hover {
  cursor: pointer;
  background: white;
  color: black;
  outline: 2px solid #000;
}

.openDiv {
  width: 100%;
  height: 100vh;
  background: #000000e7;
  position: fixed;
  top: 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  left: 0;
  z-index: 9999;
}
.imgPreview {
  width: 70%;
  object-fit: scale-down;
  max-height: 40vw;
  height: auto;
}
.prevButton,
.nextButton {
  transition: 1s linear;
  padding: 10px 35px;
  font-size: 18px;
  border: none;
  color: white;
  background: #0005;
  border-radius: 10px;
  border: 1px solid white;
  margin: 10px;
}
.prevButton:hover,
.nextButton:hover {
  background: #fff;
  color: black;
}

/* responsive CSS Code */

@media (max-width: 1199px) {
  .section-padding {
    padding-top: 70px;
  }
}
@media (max-width: 991px) {
  .section-padding {
    padding-top: 50px;
  }
}
@media (max-width: 767px) {
  .title {
    font-size: 36px;
  }
  .gallery img {
    margin: 8px 8px;
    width: 175px;
  }
  .closeBtn {
    padding: 6px 25px;
  }
  .prevButton,
  .nextButton {
    font-size: 18px;
    padding: 8px 25px;
  }
}

@media (max-width: 540px) {
  .section-padding {
    padding-top: 30px;
  }

  .gallery img {
    margin: 8px 6px;
    width: 155px;
  }

  .closeBtn {
    font-size: 18px;
    border-radius: 15px;
  }
  .prevButton,
  .nextButton {
    font-size: 18px;
    padding: 6px 20px;
    border-radius: 10px;
    margin: 5px;
  }

  .imgPreview {
    width: 90%;
    max-height: 50vh;
    height: auto;
  }
}
</style>