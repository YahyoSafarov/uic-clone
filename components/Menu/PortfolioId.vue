<template>
  <div class="container py-56">
    <div class="relative bg w-full h-full rounded-[20px] py-7">
      <div class="hero_id">
        <div>
          <div class="flex justify-between items-center p-10">
            <img src="https://uic.group/media/portfolio/logo/uzbekistans-club-logo_qIjphFx.svg" alt="no image">
            <ul class="flex gap-6 text-white text-[14px] items-center">
              <li>JAVASCRIPT (VUE.JS)</li>
              <li>PYTHON (DJANGO)</li>
              <li class="border p-[8px] text-[] w-[100px] rounded-[12px] border-[#00a795]">WEBSITE</li>
            </ul>
          </div>

          <div class="absolute w-[1350px] rounded-[12px] overflow-hidden -ml-[46px] bg_shadow">
            <div class="flex flex-col items-start justify-center ml-12 p-14">
              <h1 class="text-[#fff] font-bold text-[35px]">Uzbekistan's Club</h1>
              <p class="text-[#00a795]">Uzbekistan's Club</p>
            </div>

          </div>


          <div class="button-group mt-[200px] p-10">

            <NuxtLink to="https://uzbekistans.club/" target="_blank" class="button button-arrow bg-blue flex items-center gap-5">
              Go to the site
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
            </div>

          </div>
          <div>
            <div class="overflow-hidden mt-6" >
              <img src="https://uic.group/media/cache/b3/d7/b3d71bda0084119757c0f350af06f117.jpg" class="w-full h-[698.9px] duration-300 hover:scale-105"  alt="no image">
            </div>
            <div class="w-full flex items-center justify-center">
              <p class="text-start text-white p-16 whitespace-normal">The UIC Group provided services for the creation of a website and an application for Uzbekistan's club project, which was created to further promote the achievements of the great generation of Uzbekistan.</p>
            </div>

            <div class="overflow-hidden">
              <img src="https://uic.group/media/cache/d7/f0/d7f077d96381c1ef68a59c06e1e2d28a.jpg" class="w-full h-[698.9px] duration-300 hover:scale-105" alt="no image">
            </div>

            <div class="w-full flex items-center justify-center">
              <p class="text-start text-white p-16 whitespace-normal">The project "Uzbekistan's club" undertook the task of introducing the heroes who have reached heights in various areas of life, to unite compatriots from different parts of the world, and the website we created and the easy-to-use application will help to realize this task.

                Now users can follow the news and view media content on the platform in an easy-to-use format. The application "Uzbekistan's club" is developed for two platforms - iOS and Android.</p>
            </div>

            <div class="overflow-hidden mt-14">
              <img src="https://uic.group/media/cache/fe/cc/fecc7259ed45d7283aab7433f3e46a1f.jpg" class="w-full h-[698.9px] duration-300 hover:scale-105" alt="no image">
            </div>
          </div>

        </div>
      </div>
    </div>
  </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>
.container{
  max-width: 1310px;
}
.bg{
  background-color: #242425;
}
.hero_id{
  color: var(--cadet-gray);
  text-align: center;
  padding-block-end: 0;
  overflow: hidden;
}


.bg_shadow{
  background-color: rgba(0, 0, 0, 0.4);
  -webkit-backdrop-filter: blur(20px);
  backdrop-filter: blur(20px);
  padding-block: 20px;
  box-shadow: var(--shadow-1);
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
  .bg_shadow{
    display: none;
  }
}

</style>