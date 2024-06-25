<template>
  <div class="bg-[#000] mt-64">
    <main>
      <div class="container">

        <div class="flex items-center justify-between text_h3" data-aos="fade-up">
          <div class="" data-aos="fade-right">
            <h3 class="text-[50px] font-bold text-white">PORTFOLIO</h3>
          </div>
          <div id="btncontainer" class="filter">
            <button :class="{ 'btn-active': activeFilter === 'all' }" class="btn" @click="filterGallery('all')">
              <NuxtLink to="/portfolio">Branding</NuxtLink>
            </button>
            <button :class="{ 'btn-active': activeFilter === 'Bollywood' }" class="btn" @click="filterGallery('Bollywood')">
              <NuxtLink to="/portfolio">Mobile App</NuxtLink>
            </button>
            <button :class="{ 'btn-active': activeFilter === 'Hollywood' }" class="btn" @click="filterGallery('Hollywood')">
              <NuxtLink to="/portfolio">CRM</NuxtLink>
            </button>
            <button :class="{ 'btn-active': activeFilter === 'tv' }" class="btn" @click="filterGallery('tv')">
              <NuxtLink to="/portfolio">Website</NuxtLink>

            </button>
          </div>
        </div>

        <div id="gallery" class="photos-grid-container gallery"   data-aos="fade-up">
          <div class="main-photo img-box">
            <NuxtLink>
              <div class="col-md-6 col-lg-4">
                <div class="item animated wow fadeIn">
                  <div class="uzb_img">
                    <img src="https://uic.group/media/cache/0c/39/0c392b9a99ead3fb208087f2a1e1e145.jpg" class="" alt="no image/">
                  </div>

                  <div class="absolute -mt-56 top-10 right-[310px] z-50">
                    <p class="text-white font-bold text-[35px]">Uzbekistan's Club</p>
                    <p class="text-[#c5bebe] text-[14px]">WEBSITE</p>
                  </div>

                  <div class="overlay fade-overlay">
                    <div class="text">VIEW MORE</div>
                  </div>
                </div>
              </div>
            </NuxtLink>

          </div>
          <div>
            <div class="sub">
              <div v-for="index in images" :key="index"

              >
                <div class="img-box">
                  <NuxtLink data-aos="fade-right">
                    <div class="col-md-6 col-lg-4">
                      <div class="item animated wow fadeIn">
                        <img :src="index.src" class="rounded-[12px]" alt="no image">
                        <div class="absolute top-0 left-5 z-50">
                          <p class="text-white font-bold text-[25px]">{{index.titleabs}}</p>
                          <p class="text-[#c5bebe] text-[14px]">WEBSITE</p>
                        </div>
                        <div class="overlay fade-overlay">
                          <div class="text2">VIEW MORE</div>
                        </div>
                      </div>
                    </div>
                  </NuxtLink>
                </div>
              </div>

              <div id="multi-link" class="img-box">

              </div>
            </div>

          </div>

        </div>

        <div id="gallery" class="photos-grid-container gallery" data-aos="fade-up">
          <div class="main-photo img-box">
            <NuxtLink data-aos="fade-right">
              <div class="col-md-6 col-lg-4">
                <div class="item animated wow fadeIn">
                  <div class="uzb_img">
                    <img src="https://uic.group/media/cache/77/4d/774ddc33fda844b44bb597539531dec6.jpg" class="" alt="no image/">
                  </div>

                  <div class="absolute -mt-56 top-10 left-10 z-50">
                    <p class="text-white font-bold text-[35px]">WAYU</p>
                    <p class="text-[#c5bebe] text-[14px]">WEBSITE</p>
                  </div>

                  <div class="overlay fade-overlay">
                    <div class="text">VIEW MORE</div>
                  </div>
                </div>
              </div>
            </NuxtLink>

          </div>
          <div>
            <div class="sub">
              <div v-for="index in serviceimg" :key="index"
              >
                <div class="img-box">
                  <NuxtLink>
                    <div class="col-md-6 col-lg-4">
                      <div class="item animated wow fadeIn">
                        <img :src="index.src" class="rounded-[12px]" alt="no image">
                        <div class="absolute top-0 left-5 z-50">
                          <p class="text-white font-bold text-[25px]">{{index.titleabs}}</p>
                          <p class="text-[#c5bebe] text-[14px]">WEBSITE</p>
                        </div>
                        <div class="overlay fade-overlay">
                          <div class="text2">VIEW MORE</div>
                        </div>
                      </div>
                    </div>
                  </NuxtLink>
                </div>
              </div>

              <div id="multi-link" class="img-box">

              </div>
            </div>
          </div>
          <div class="button-group">

            <NuxtLink to="/portfolio" class="button button-arrow bg-blue flex items-center gap-5 cursor-pointer">
              All Projects
              <svg viewBox="0 0 6 9" fill="none" xmlns="http://www.w3.org/2000/svg" class="arrow-icon">
                <g class="arrow-head">
                  <path d="M1 1C4.5 4 5 4.38484 5 4.5C5 4.61516 4.5 5 1 8" stroke="currentColor" stroke-width="2"/>
                </g>
                <g class="arrow-body">
                  <path d="M3.5 4.5H0" stroke="currentColor" stroke-width="2"/>
                </g>
              </svg>
            </NuxtLink>

          </div>
        </div>

      </div>
    </main>
  </div>
</template>

<script setup>

import {onMounted} from "vue";
import AOS from 'aos';
import 'aos/dist/aos.css'


const images = ref([
      {
        id: 1,
        src: 'https://uic.group/media/cache/29/88/29883e26588ac429b3ca86b3ac39efa6.jpg',
        category: 'Bollywood',
        title1: "theBEVERLY",
        titleabs: "Anatomica",
        mintitle1: "Salt Lake City",
        title2: "Now Leasing",
        mintitle2: "Apartments / Starting From — $1,675+ Monthly",
      },
      {
        id: 2,
        src: 'https://uic.group/media/cache/cc/39/cc392cc7e6083d974df22bdf3f7baae3.jpg',
        category: 'Bollywood',
        title1: "theBEVERLY",
        titleabs: "Anatomica App",
        mintitle1: "Salt Lake City",
        title2: "Now Leasing",
        mintitle2: "Apartments / Starting From — $1,675+ Monthly",
      },
      {
        id: 3,
        src: 'https://uic.group/media/cache/59/f1/59f1ca58bab7263f9c5eaff3033d5951.jpg',
        category: 'Bollywood',
        title1: "theBEVERLY",
        titleabs: "Express 24",
        mintitle1: "Salt Lake City",
        title2: "Now Leasing",
        mintitle2: "Apartments / Starting From — $1,675+ Monthly",
      },
      {
        id: 4,
        src: 'https://uic.group/media/cache/b6/27/b6273a3cbd3fe1e5ad0e9b9acdccdfc4.jpg',
        category: 'Bollywood',
        title1: "theBEVERLY",
        titleabs: "Toshkent Parfum",
        mintitle1: "Salt Lake City",
        title2: "Now Leasing",
        mintitle2: "Apartments / Starting From — $1,675+ Monthly",
      },
    ],
);



const serviceimg = ref([
      {
        id: 1,
        src: 'https://uic.group/media/cache/b3/6b/b36bc02390ec157e4a4a99eb5c0643b2.jpg',
        category: 'Bollywood',
        title1: "theBEVERLY",
        titleabs: "Anatomica",
        mintitle1: "Salt Lake City",
        title2: "Now Leasing",
        mintitle2: "Apartments / Starting From — $1,675+ Monthly",
      },
      {
        id: 2,
        src: 'https://uic.group/media/cache/cc/39/cc392cc7e6083d974df22bdf3f7baae3.jpg',
        category: 'Bollywood',
        title1: "theBEVERLY",
        titleabs: "Uzbekistan's club App",
        mintitle1: "Salt Lake City",
        title2: "Now Leasing",
        mintitle2: "Apartments / Starting From — $1,675+ Monthly",
      },
      {
        id: 3,
        src: 'https://uic.group/media/cache/30/da/30da918dacc113dd034fb5dbb8063282.jpg',
        category: 'Bollywood',
        title1: "theBEVERLY",
        titleabs: "Ricomel",
        mintitle1: "Salt Lake City",
        title2: "Now Leasing",
        mintitle2: "Apartments / Starting From — $1,675+ Monthly",
      },
      {
        id: 4,
        src: 'https://uic.group/media/cache/d4/e7/d4e7073d362f8d5a16efbb3e656fc4ee.jpg',
        category: 'Bollywood',
        title1: "theBEVERLY",
        titleabs: "Infomax freight",
        mintitle1: "Salt Lake City",
        title2: "Now Leasing",
        mintitle2: "Apartments / Starting From — $1,675+ Monthly",
      },
    ],
);

onMounted(() => {
  AOS.init ({
    duration: 1000,
    easing: 'ease-in-out',
    once: true,
  })
})


</script>

<style lang="scss" scoped>
.bg{
  background: #0c0c0c;
  //background-color: black;
}

@import url("https://fonts.googleapis.com/css2?family=Raleway:wght@500&display=swap");



* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

h1 {
  font-size: 1.2rem;
}



.photos-grid-container {
  height: 100%;
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr;
  grid-gap: 2rem;
  justify-content: center;
  align-items: start;
  margin-top: 20px;

  @media (max-width: 580px) {
    grid-template-columns: 1fr;
  }

  .img-box {
    //border: 1px solid #ffffff;
    position: relative;
  }

  .img-box img{
    width: 370px;
    height: 220px;
  }



  .img-box:hover .caption {
    transform: translateY(-5px);
  }

  img{
    max-width: 100%;
    display: block;
    height: auto;
    filter: brightness(60%);
  }

  .uzb_img img{
    width: 700px;
    height: 457px;
  }

  .caption {
    color: white;
    transition: transform 0.3s ease, opacity 0.3s ease;
    font-size: 1.5rem;
  }

  .transparent-box {
    height: 100%;
    width: 100%;

    position: absolute;
    top: 0;
    left: 0;
    transition: background-color 0.3s ease;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .main-photo {
    grid-row: 1;
    grid-column: 1;
  }

  .sub {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 1fr 1fr;
    grid-gap: 1.5em;

    &:nth-child(0) {
      grid-column: 1;
      grid-row: 1;
    }

    &:nth-child(1) {
      grid-column: 2;
      grid-row: 1;
    }

    &:nth-child(2) {
      grid-column: 1;
      grid-row: 2;
    }

    &:nth-child(3) {
      grid-column: 2;
      grid-row: 2;
    }
  }
}


.hide-element {
  border: 0;
  clip: rect(1px 1px 1px 1px); /* IE6, IE7 */
  clip: rect(1px, 1px, 1px, 1px);
  height: 1px;
  margin: -1px;
  overflow: hidden;
  padding: 0;
  position: absolute;
  width: 1px;
}


.overlay {
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  background:
      linear-gradient(160deg, rgba(45, 184, 147, 0.64), rgba(45, 184, 147, 0.20), rgba(67, 67, 67, 0.10), rgba(45, 184, 147, 0.94),);
  overflow: hidden;
  width: 100%;
  height: 100%;
  transition: .5s ease;
  border-radius: 12px;
  cursor: pointer;
}

.item {
  position: relative;
  overflow: hidden;

}

.item:hover .overlay {
  bottom: 0;
  height: 100%;
  width: 100%;
}

.top-overlay {
  bottom: 100%;
  height: 0;
}
.item:hover .top-overlay {
  bottom: 0;
}
.bottom-overlay {
  top: 100%;
}

.item:hover .bottom-overlay {
  top: 0;
}

.right-overlay {
  left: 100%;
  height: 100%;
}

.item:hover .right-overlay {
  left : 0;
}

.left-overlay {
  right: 100%;
  height: 100%;
  left:auto;
}

.item:hover .left-overlay {
  right : 0;
}
.fade-overlay {
  height: 100%;
  opacity: 0;
}

.item:hover .fade-overlay {
  opacity: 1;
}
.title-overlay {
  height: auto;
  top: auto;
  opacity: 0;
}
.item:hover .title-overlay {
  opacity: 1;
  height: auto;
  padding: 50px 0;
}
.text {
  color: white;
  font-size: 1.2vw;
  position: absolute;
  top: 90%;
  left: 77%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
  font-weight: 700;
}
.text2 {
  color: white;
  font-size: 1.2vw;
  position: absolute;
  top: 90%;
  left: 60%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
  font-weight: 700;
}



.filter {
  text-align: center;
  max-width: 1050px;
}

text_h3{
  margin-bottom: 80px;
}

.btn {
  padding: 10px 20px;
  margin: 7px 6px 6px 0;
  display: inline-block;
  color: #c5bebe;
  background: transparent;
  border: 2px solid #636060;
  transition: all 0.4s;
  border-radius: 10px;
  font-size: 16px;
  font-weight: 500;
}
.btn:hover, .btn-active {
  border: 2px solid #00a795;
  color: #00a795;
  transform: translateY(3px);
}


$button-transition-timing: 100ms;
.button-group {
  display: flex;
  gap: 10px;
  position: relative;
  z-index: 999;
  margin-bottom: 40px;
}

.button {
  border-radius: 12px;
  color: #333;
  font-weight: bold;
  padding: 10px 30px;
  text-decoration: none;
  transition: all $button-transition-timing ease-in-out;

  &:hover {
    background-color: #e6e6e6;
  }

  &:not(:first-of-type) {
    margin-left: 15px;
  }

  &.bg-blue {
    background-color: #1a8377;
    border: 2px solid #00a795;
    color: #fff;

    &:hover {
      background-color: #00a795;
    }
  }
}

.button-arrow {

  .arrow-icon {
    overflow: visible;
    margin-left: 3px;
    width: 8px;
  }

  .arrow-head {
    transform: translateX(0);
    transition: transform $button-transition-timing ease-in-out;
  }

  .arrow-body {
    opacity: 0;
    transform: scaleX(1);
    transition: transform $button-transition-timing ease-in-out, opacity $button-transition-timing ease-in-out;
  }

  &:hover {
    .arrow-head {
      transform: translateX(3px);
    }

    .arrow-body {
      opacity: 1;
      transform: scaleX(2);
    }
  }

}

.btn__call{
  backdrop-filter: blur(20px);
  border-radius: 12px;
  border: 2px solid #ffffff;
  padding: 10px 30px;
  transition-duration: 0.5s;

  &:hover{
    background-color: #00a795;
    border: 2px solid #00a795;
    box-shadow: 0 0 10px #00a795;
  }
}




@media screen and (min-width: 1280px) {

  .container {
    margin: 10px auto;
    width: 1300px;
    padding-top: 80px;
  }
}

</style>
