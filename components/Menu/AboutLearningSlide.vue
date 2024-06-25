<template>
  <div class="container">
    <div class="">
      <div class="logos bg-[#262727] rounded-[12px]">
        <div class="p-12">
          <h1 class="text-white text-[25px] font-bold">The Co-learning Center is a friend of UIC</h1>
        </div>
        <swiper
            :slidesPerView="3.5"
            :autoplay="{
          delay: 2500,
          disableOnInteraction: false,
          }"
            :scrollbar="{
              hide: true,
              bacground: '#fff',
            }"
            :spaceBetween="25"
            :modules="modules"
            class="mySwiper cursor-pointer"
        >
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/assets/senter1.ffdd962a.jpg" alt="no image">
                <div class="overlay fade-overlay">
                  <!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/assets/senter7.5480cf52.jpg" alt="no image">
                <div class="overlay fade-overlay">
                  <!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/assets/senter2.967d5c4f.jpg" alt="no image">
                <div class="overlay fade-overlay">
                  <!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>

          </swiper-slide>

          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/assets/senter6.aee5389c.jpg" alt="no image">
                <div class="overlay fade-overlay">
                  <!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>

          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/assets/senter4.10fb5d27.jpg" alt="no image">
                <div class="overlay fade-overlay">
                  <!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>

          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/assets/senter5.66af7fc7.jpg" alt="no image">
                <div class="overlay fade-overlay">
                  <!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>

          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/assets/senter3.da41edb3.jpg" alt="no image">
                <div class="overlay fade-overlay">
                  <!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>

          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/assets/senter8.ad6b4d50.jpg" alt="no image">
                <div class="overlay fade-overlay">
                  <!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>

          </swiper-slide>
        </swiper>
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
import 'swiper/css/navigation';


// import required modules
import {Scrollbar, Autoplay, Pagination, Navigation } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [ Scrollbar, Autoplay, Pagination, Navigation],
    };
  },
};
</script>


<style scoped>
.container{
  max-width: 1170px;
}
.mySwiper{
  padding: 25px;
  border-radius: 15px;
  color: white;
}
.logos:before {
  left: 0;
  background: linear-gradient(to left, rgba(255, 255, 255, 0), #070a0e);
}

.logos:after {
  right: 0;
  background: linear-gradient(to right, rgba(255, 255, 255, 0), #23415d);
}
.swiper {
  width: 100%;
  height: 100%;
}



.swiper-slide {
  text-align: center;
  font-size: 18px;

  /* Center slide text vertically */
  display: flex;
  justify-content: center;
  align-items: center;
}

.swiper-slide img {
  display: block;
  width: 350px;
  height: 200px;
  object-fit: cover;
  border-radius: 16px;
}

.swiper {
  margin-left: auto;
  margin-right: auto;
}

.swiper-scrollbar-drag{
  height: 100%;
  width: 100%;
  position: relative;
  background: rgba(221, 26, 26, 0.5);
  border-radius: 10px;
  left: 0;
  top: 0;
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
  margin: 10px 0;
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



mySwiper.swiper-scrollbar-drag {
  height: 100%;
  width: 100%;
  position: relative;
  background: rgba(236, 30, 30, 0.5);
  border-radius: 10px;
  left: 0;
  top: 0;
}
</style>


