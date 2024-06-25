<template>
  <div class="container">
    <div class="mt-44">
      <div class="logos">
        <swiper
            :slidesPerView="3.5"
            :autoplay="{
          delay: 2500,
          disableOnInteraction: false,
          }"
            :scrollbar="{
              hide: true,
              color: '#fff',
            }"
            :spaceBetween="25"
            :loop="true"
            :modules="modules"
            class="mySwiper cursor-pointer"
        >
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/media/cache/4a/9f/4a9ff516211f69f069ed456755ca71c9.jpg" alt="no image">
                <div class="overlay fade-overlay">
<!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/media/cache/4a/9f/4a9ff516211f69f069ed456755ca71c9.jpg" alt="">
                <div class="overlay fade-overlay">
<!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/media/cache/de/7c/de7c4a35b647de3c865213ddd9706d16.jpg" alt="">
                <div class="overlay fade-overlay">
<!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>

          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/media/cache/d0/5f/d05f677daed2f3281207e49a6130b893.jpg" alt="">
                <div class="overlay fade-overlay">
<!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>

          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/media/cache/29/bb/29bbc6b12276f94f2f18b62a10f51545.jpg" alt="">
                <div class="overlay fade-overlay">
<!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>

          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/media/cache/00/c7/00c70d8f67985fcd0aabfebd070f9930.jpg" alt="">
                <div class="overlay fade-overlay">
<!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>

          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/media/cache/00/a1/00a167617347354585ec74142a8120fd.jpg" alt="">
                <div class="overlay fade-overlay">
<!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>

          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/media/cache/9a/d7/9ad7e189c895f399a6f4330eacb3f041.jpg" alt="">
                <div class="overlay fade-overlay">
<!--                  <div class="text">Fade in overlay</div>-->
                </div>
              </div>
            </div>

          </swiper-slide>
          <swiper-slide>
            <div class="col-md-6 col-lg-4">
              <div class="item animated wow fadeIn">
                <img src="https://uic.group/media/cache/9a/d7/9ad7e189c895f399a6f4330eacb3f041.jpg" alt="">
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

<!--<script setup>-->
<!--const image = [-->
<!--  {-->
<!--    id: 1,-->
<!--    img: "https://uic.group/media/cache/4a/9f/4a9ff516211f69f069ed456755ca71c9.jpg",-->
<!--  },-->
<!--  {-->
<!--    id: 2,-->
<!--    img: "https://uic.group/media/cache/4a/9f/4a9ff516211f69f069ed456755ca71c9.jpg",-->
<!--  },-->
<!--  {-->
<!--    id: 3,-->
<!--    img: "https://uic.group/media/cache/4a/9f/4a9ff516211f69f069ed456755ca71c9.jpg",-->
<!--  },-->
<!--  {-->
<!--    id: 4,-->
<!--    img: "https://uic.group/media/cache/4a/9f/4a9ff516211f69f069ed456755ca71c9.jpg",-->
<!--  },-->
<!--  {-->
<!--    id: 5,-->
<!--    img: "https://uic.group/media/cache/4a/9f/4a9ff516211f69f069ed456755ca71c9.jpg",-->
<!--  },-->
<!--]-->
<!--</script>-->

<style scoped>
.container{
  max-width: 1320px;
}
.swiper-scrollbar-drag{
  background: #00a795 !important;
}
.mySwiper{
  background: #262727;
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
</style>


