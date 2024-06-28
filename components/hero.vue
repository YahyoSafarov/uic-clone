<template>
  <div class="bg_image">

    <!--
      - #HERO
    -->

    <section class="section hero" id="home" aria-label="hero" data-section
             style="background-image: url('../assets/images/uic-group-main_back.webp')">
      <div class="container">

        <div class="hero-content">


          <div class="text-[440px] font-bold">
            <h1 class="headline -mt-[120px] -ml-[45px]">
              <svg aria-hidden="true" id="lockup-headline-mask" class="headline lockup-headline-mask visually-hidden">
                <clipPath id="lockup-headline-mask-path">
                  <text dominant-baseline="hanging" text-anchor="middle" x="75%" y="em" dy="0.125em">UIC</text>
                </clipPath>
              </svg>
            </h1>
          </div>

          <div class="container media_text">
            <div class="relative z-50 flex justify-start flex-col items-start gap-4 -mt-36">
              <p class="text-white font-[700] text-[54px] text-start">
                We offer digital <br> solutions
              </p>
              <p class="text-gray-300 font-bold text-[22px] mb-10">
                IN ANY DIFFICULTY
              </p>
            </div>
            <div class="button-group">

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

          <div class="flex justify-center items-center">
            <img src="https://uic.group/uic-images/mountain.webp" class="absolute max-w-full w-[100%] top-[180px] f_image"  alt="no image">
          </div>

        </div>



        <div class="circle">
          <div class="logo"></div>
          <div class="text">
            <p>I never tell the same joke twice I have a DRY sense of humor.</p>
          </div>
        </div>

<!--        More components-->
<!--        <div x-show="open" class="fixed bottom-0 right-0 w-full md:bottom-8 md:right-12 md:w-auto z-50" x-data="{ open: true }">-->
<!--          <div class="bg-gray-800 text-gray-50 text-sm p-3 md:rounded shadow-lg flex justify-between">-->
<!--            <div>👉 <a class="hover:underline ml-1" href="https://cruip.com/?ref=codepen-cruip-blog-post-hover" target="_blank">More components on Cruip.com</a></div>-->
<!--            <button class="text-gray-500 hover:text-gray-400 ml-5" @click="open = false">-->
<!--              <span class="sr-only">Close</span>-->
<!--              <svg class="w-4 h-4 flex-shrink-0 fill-current" viewBox="0 0 16 16">-->
<!--                <path d="M12.72 3.293a1 1 0 00-1.415 0L8.012 6.586 4.72 3.293a1 1 0 00-1.414 1.414L6.598 8l-3.293 3.293a1 1 0 101.414 1.414l3.293-3.293 3.293 3.293a1 1 0 001.414-1.414L9.426 8l3.293-3.293a1 1 0 000-1.414z" />-->
<!--              </svg>-->
<!--            </button>-->
<!--          </div>-->
<!--        </div>-->
<!--        <div class="hero-banner">-->

<!--          <img src="./assets/images/hero-banner.png" width="660" height="753" alt="hero banner" class="w-100">-->

<!--          <img src="./assets/images/hero-circle-one.png" width="666" height="666" aria-hidden="true" alt=""-->
<!--               class="circle circle-1">-->
<!--          <img src="./assets/images/hero-circle-two.png" width="666" height="666" aria-hidden="true" alt=""-->
<!--               class="circle circle-2">-->

<!--          <img src="./assets/images/heart-rate.svg" width="255" height="270" alt="heart rate"-->
<!--               class="abs-img abs-img-1">-->
<!--          <img src="./assets/images/calories.svg" width="348" height="224" alt="calories" class="abs-img abs-img-2">-->

<!--        </div>-->

      </div>

    </section>
  </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.bg_image{
  background-image: linear-gradient(to left, rgba(0,0,0,0.4),rgba(0,0,0,0.3)), url("../assets/images/uic-group-main_back.webp");
  width: 100%;
  height: 100vh;
  background-size: cover;
  background-position: center;
}

.f_image{
  filter: brightness(60%);
}

/*-----------------------------------*\
  #HERO
\*-----------------------------------*/

.hero {
  color: var(--cadet-gray);
  text-align: center;
  padding-block-start: calc(var(--section-padding) + 80px);
  padding-block-end: 0;
  overflow: hidden;
}

.hero::after {
  bottom: 0;
  left: 0;
  width: 100%;
  height: 240px;
  background-color: var(--coquelicot);
  z-index: -1;
}

.hero-content { margin-block-end: 90px; }

.hero-subtitle {
  background-color: var(--white_10);
  color: var(--white);
  margin-inline: auto;
  padding: 5px;
  padding-inline-end: 15px;
  border-radius: var(--radius-8);
}

.hero-subtitle .strong {
  display: inline-block;
  background-color: var(--coquelicot);
  padding: 2px 15px;
  margin-inline-end: 15px;
  border-radius: var(--radius-5);
}

.hero-title { margin-block: 30px 8px; }

.hero .section-text { margin-block-end: 40px; }

.hero .btn { margin-inline: auto; }

.hero-banner { position: relative; }

.abs-img-1 {
  top: 20px;
  right: -50px;
  width: 190px;
}

.abs-img-2 {
  bottom: -50px;
  left: -40px;
  width: 280px;
}

.hero .abs-img { animation: move 3s linear infinite alternate; }

@keyframes move {
  0% { transform: translate(0, 0); }
  50% { transform: translate(-5px, 10px); }
  100% { transform: translate(5px, 20px); }
}

.hero .abs-img-2 { animation-direction: alternate-reverse; }



h1 {
  position: relative;
  color: white;
}
.headline {
  width: 100%;
  font: 25vw system-ui, sans-serif;
  font-weight: 900;
  height: 450px;
}
@supports (backdrop-filter: blur(10px)) {
  .visually-hidden {
    position: absolute;
    top: -9999px;
    left: -9999px;
  }
  h1 {
    backdrop-filter: blur(12px);
    background: rgba(white, 0.4);
    clip-path: url(#lockup-headline-mask-path);
  }
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

@media(max-width: 1200px){
  .f_image{
    display: none;
  }
  .headline{
    margin-left: -250px;
  }
  .media_text{
    display: flex;
    flex-direction: column;
    margin-top: -100px;
    align-items: center;
    justify-content: center;
  }
}
</style>



