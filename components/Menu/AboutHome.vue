<template>
  <div class="bg">
    <div class="hero">
      <div class="container" data-aos="fade-up">
        <div class="flex items-center justify-center mt-32" data-aos="zoom-in">
          <img src="https://uic.group/uic-images/about/about-uic-logo.png" class="w-full max-w-[650px]" alt="no image">
        </div>

        <div>
          <div v-for="item in text" :key="item"
          >
            <div class="flex flex-col items-start justify-start text-start mt-20">
              <h2 class="text-white text-[25px] font-bold">{{item.name}}</h2>
              <div class="flex flex-col gap-10 text-[15px]">
                <p class="text-white">{{item.title}}</p>
                <p class="text-white">{{item.title2}}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script setup>
import {onMounted} from "vue";
import AOS from 'aos';
import 'aos/dist/aos.css'

const text = [
  {
    id: 1,
    name: "About UIC",
    title: "“United IT Company” was founded on October 8, 2020. According to the director of the company Murodkhuja Muratov, the philosophy of the company is to create a team that meets international standards in the IT field of Uzbekistan, to open up the opportunity for young programmers to work on themselves and at the same time be officially employed, to bring the company to a prominent place in the world arena IT.",
    title2: "At the time the company was founded, the team consisted of only 10 people, and now the team has +100 specialists. These people believed in the philosophy of the company and sought to contribute to the development of the project. To this day, these people remain loyal to the company and develop their teams within the company in different directions (Backend, Frontend, QA, Mobile, Analytics, Marketing Team, etc.).",
  }
]

onMounted(() => {
  AOS.init ({
    duration: 1000,
    easing: 'ease-in-out',
    once: true,
  })
})
</script>

<style lang="scss" scoped>
.container{
  max-width: 1170px;
}
.bg{
  background-image: linear-gradient(to top, rgba(0,0,0,0.2), rgba(0, 255, 225, 0.1));
  width: 100%;
  height: 100vh;
  background-size: cover;
  background-position: center;
}
.hero{
  color: var(--cadet-gray);
  text-align: center;
  padding-block-start: calc(var(--section-padding) + 80px);
  padding-block-end: 0;
  overflow: hidden;
}
</style>