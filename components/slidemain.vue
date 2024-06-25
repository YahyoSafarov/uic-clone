<template>
  <div class="container py-36 mt-64">
    <div class="hero">
      <div class="grid grid-cols-1 items-center sm:grid-cols-2 gap-8 grid_media">
        <div class="flex gap-14 items-center ml-14 justify-center media_flex">
          <swiper
              :autoplay="{
      delay: 2500,
      disableOnInteraction: false,
    }"
              :modules="modules"
              class="mySwiper -mt-56"
          >
            <div>

            </div>
            <swiper-slide class="">
              <div class="col-md-6 col-lg-4">
                <div class="item animated wow fadeIn">
                  <img src="https://uic.group/media/cache/5a/70/5a70d134e3000c5ef605393b360f73fe.jpg" alt="">
                  <div class="overlay fade-overlay">
                    <div class="text">Fade in overlay</div>
                  </div>
                </div>
              </div>
            </swiper-slide>
            <swiper-slide class="mb-2">
              <div class="col-md-6 col-lg-4">
                <div class="item animated wow fadeIn">
                  <img src="https://uic.group/media/cache/21/e5/21e58126b6c478060b6e6fd54ca6fbba.jpg"  alt="">
                  <div class="overlay fade-overlay">
                    <div class="text">Fade in overlay</div>
                  </div>
                </div>
              </div>
            </swiper-slide>

            <div class="border-b-[2px] border-[#999999] media_border"></div>
            <div class="flex text-start items-center gap-4 mt-2">
              <p class="text-[50px] font-bold text-white">10</p>
              <p class="text-[15px] font-[600] text-[#00a795] leading-8">ANNUAL <br> QUALIFICATION TEAM</p>
            </div>
          </swiper>

          <swiper
              :autoplay="{
      delay: 2500,
      disableOnInteraction: false,
    }"
              :modules="modules"
              class="mySwiper swipe_img"
          >
            <swiper-slide>
              <div class="col-md-6 col-lg-4">
                <div class="item animated wow fadeIn">
                  <img src="https://uic.group/media/cache/1c/ac/1cac8a7441794ad91f2cc94093c84fd0.jpg" alt="">
                  <div class="overlay fade-overlay">
                    <div class="text">Fade in overlay</div>
                  </div>
                </div>
              </div>

            </swiper-slide>
            <swiper-slide>

              <div class="col-md-6 col-lg-4">
                <div class="item animated wow fadeIn">
                  <img src="https://uic.group/media/cache/63/2a/632ae021916378d650ff3ffb98fcb7c1.jpg"  alt="">
                  <div class="overlay fade-overlay">
                    <div class="text">Fade in overlay</div>
                  </div>
                </div>
              </div>

            </swiper-slide>
          </swiper>
        </div>
        
        <div class="container pl-20">
          <div class="flex flex-col items-start justify-start gap-6">
            <div class="flex items-center gap-6 ">
              <div class="border-t-[2px] border-[#999999] w-[30px]"></div>
              <h2 class="text-[#00a795] font-bold text-[16px]">IN THE WORLD</h2>
            </div>
            <div class="flex flex-col justify-start items-start">
              <h1 class="font-bold text-white text-[50px]">About us</h1>
              <p class="text-start mb-4 text-[16px] text-[#999]">
                Every big company needs to thank not only itself, but also those who have stood beside it and believed in it. After all, the most important principle in our work is trust.
              </p>

              <p class="text-start text-[16px] text-[#999]">
                Trust not only ensures the loyalty of customers and partners, but also increases our demand for ourselves. We cooperate on the basis of relations built on thousand-year human traditions.
              </p>

              <div class=" flex gap-56 mt-14">
                <div class="flex items-center gap-6">
                  <i data-v-56c03d90="" data-v-77920e16="" class="icon hover:text-red-500 text-[#00A795] mr-1"><svg width="26" height="46" viewBox="0 0 26 46" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M12.8913 20.1951L22.1404 21.0359L13.5412 38.2342L14.1979 27.0704C14.236 26.4237 13.7538 25.8636 13.1086 25.8049L3.85958 24.9641L12.4588 7.76573L11.8021 18.9295C11.764 19.5762 12.2462 20.1364 12.8913 20.1951ZM24.1086 18.8049L14.2662 17.9101L15.1979 2.07045C15.2745 0.767755 13.5103 0.296146 12.9267 1.46332L0.92668 25.4633C0.548736 26.2192 1.04971 27.1185 1.89135 27.1951L11.7338 28.0898L10.8021 43.9295C10.7254 45.2322 12.4897 45.7038 13.0733 44.5366L25.0733 20.5366C25.4513 19.7808 24.9503 18.8814 24.1086 18.8049Z" fill="#00A795" stroke="#00A795" stroke-width="0.4"></path>
                  </svg>
                  </i>
                  <p class="text-start text-[#999] font-medium text-[16px]">Quick <br> solutions</p>
                </div>

                <div class="flex items-center gap-6">
                  <i data-v-56c03d90="" data-v-77920e16="" class="icon hover:text-red-500 text-[#00A795] mr-1"><svg width="48" height="48" viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M30 15.5C30 16.0523 30.4477 16.5 31 16.5H32C32.5523 16.5 33 16.0523 33 15.5V4C33 3.44772 33.4477 3 34 3H44C44.5523 3 45 3.44772 45 4V44C45 44.5523 44.5523 45 44 45H34C33.4477 45 33 44.5523 33 44V32.5C33 31.9477 32.5523 31.5 32 31.5H31C30.4477 31.5 30 31.9477 30 32.5V47C30 47.5523 30.4477 48 31 48H47C47.5523 48 48 47.5523 48 47V0.999999C48 0.447714 47.5523 0 47 0H31C30.4477 0 30 0.447715 30 1V15.5Z" fill="#00A795"></path>
                    <path d="M41 28.5C41.5523 28.5 42 28.0523 42 27.5V22.3142C42 22.049 41.8946 21.7947 41.7071 21.6071L39.8929 19.7929C39.7054 19.6054 39.451 19.5 39.1858 19.5H21.296C20.8534 19.5 20.4679 19.2066 20.3123 18.7924C18.3937 13.6861 12.8095 10.8715 7.5 12.45C3 13.8 0 17.85 0 22.5V25.5C0 31.35 4.65 36 10.5 36C14.9026 36 18.7674 33.3107 20.3119 29.2052C20.4674 28.7919 20.8524 28.5 21.294 28.5H41ZM37.9858 22.5C38.251 22.5 38.5054 22.6054 38.6929 22.7929L38.7071 22.8071C38.8946 22.9947 39 23.249 39 23.5142V24.5C39 25.0523 38.5523 25.5 38 25.5H22C21.4477 25.5 21 25.0523 21 24.5V23.5C21 22.9477 21.4477 22.5 22 22.5H37.9858ZM10.5 33C6.3 33 3 29.7 3 25.5V22.5C3 18.3 6.3 15 10.5 15C14.7 15 18 18.3 18 22.5V25.5C18 29.7 14.7 33 10.5 33Z" fill="#00A795"></path>
                    <path d="M8 21H7C6.44772 21 6 21.4477 6 22V26C6 26.5523 6.44772 27 7 27H8C8.55228 27 9 26.5523 9 26V22C9 21.4477 8.55228 21 8 21Z" fill="#00A795"></path>
                  </svg>
                  </i>
                  <p class="text-start text-[#999] font-medium text-[16px]">Unique <br> projects</p>
                </div>


              </div>

              <div class="button-group">

                <div class=" flex gap-8 mt-20">
                  <NuxtLink to="" class="button button-arrow bg-blue flex items-center gap-5">
                    Portfolio
                    <svg viewBox="0 0 6 9" fill="none" xmlns="http://www.w3.org/2000/svg" class="arrow-icon">
                      <g class="arrow-head">
                        <path d="M1 1C4.5 4 5 4.38484 5 4.5C5 4.61516 4.5 5 1 8" stroke="currentColor" stroke-width="2"/>
                      </g>
                      <g class="arrow-body">
                        <path d="M3.5 4.5H0" stroke="currentColor" stroke-width="2"/>
                      </g>
                    </svg>
                  </NuxtLink>
                  <div>
                    <NuxtLink class="flex gap-6 items-center btn__call">
                      <p class="text-white text-[16px] font-bold">Call</p>
                      <img src="../assets/images/phone-call-regular-24%20(1).png" class="w-[18px]" alt="no icon">
                    </NuxtLink>
                  </div>
                </div>


              </div>
            </div>
          </div>
        </div>
      </div>

    </div>

  </div>

</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/pagination';



// import required modules
import {Autoplay, Pagination } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Autoplay, Pagination],
    };
  },
};
</script>

<style lang="scss" scoped>

.hero {
  color: var(--cadet-gray);
  text-align: center;
  padding-block-start: calc(var(--section-padding) + 80px);
  padding-block-end: 0;
  overflow: hidden;
}
.swiper {
  width: 450px;
  height: 100%;
  //background: white;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;
  //background: #fff;
  /* Center slide text vertically */
  display: flex;
  justify-content: center;
  align-items: center;
}

.swiper-slide img {
  display: block;
  width: 750px;
  height: 500px;
  border-radius: 12px;
  object-fit: cover;
}




$button-transition-timing: 100ms;
.button-group {
  display: flex;
  gap: 10px;
  position: relative;
  z-index: 999;
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



img {
  max-width: 100%;
  height: auto;
}
section {
  padding: 60px 0;
  min-height: 100vh;
}


.blog img{
  max-width: 100%;
}
.blog-head {
  margin-bottom: 70px;
}

.blog-head h6{
  color: #f05907;
  position: relative;
  display: inline-block;
  text-transform: capitalize;
}

.blog-head h6:after, .blog-head h6:before{
  position: absolute;
  content: "";
  width: 50px;
  height: 3px;
  background: #f05907;
  top: 50%;
}

.blog-head h6:after{
  right: 120%;
}

.blog-head h6:before{
  left: 120%;
}


.overlay {
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
  background-color: rgba(45, 184, 147, 0.44);
  overflow: hidden;
  width: 100%;
  height: 100%;
  transition: .5s ease;
  border-radius: 12px;
}

.item {
  position: relative;
  overflow: hidden;
  margin: 20px 0;
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
  top: 50%;
  left: 50%;
  -webkit-transform: translate(-50%, -50%);
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  text-align: center;
}

@media(max-width: 1200px){
  .container{
    max-width: 1200px;
    padding: 8px;
  }
  .swiper{

  }
  .grid_media{
   display: flex;
    flex-direction: column;
    gap: 10px ;
  }
  .swiper-slide img {
    display: block;
    width: 350px;
    height: 500px;
    border-radius: 12px;
    object-fit: cover;
  }
  .media_flex{
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .swipe_img{
  }
  .media_border{
    display: none;
  }
}

@media(max-width: 650px){
  .media_flex{
    display: flex;
    align-items: start;
    flex-direction: column;
    justify-content: start;
  }
}

</style>


