<template>
  <div class="container py-64">

    <div v-if="!isLoaded" class="overlay">
      <div class="overlayDoor"></div>
      <div class="overlayContent">
        <div class="loader">
          <div class="inner"></div>
        </div>
        <!--        <div class="skip" @click="skipLoading">SKIP</div>-->
      </div>
    </div>

    <div data-aos="fade-up">
      <div data-aos="fade-right">
        <div class="flex items-center gap-6 ">
          <h2 class="text-[#00a795] font-bold text-[16px]">IS THERE A PROBLEM?</h2>
        </div>
        <h2 class="text-white font-bold text-[45px] mb-10">What solution do you want?</h2>
      </div>

    </div>

    <div class="">
      <div class="grid grid-cols-2 gap-10 place-items-center">
        <div
            v-for="index in services"
            :key="index"
            data-aos="fade-up"
        >
          <div
              class="bg-[#252525] flex flex-col w-full h-[180px] p-10 rounded-[12px] duration-300 hover:shadow-2xl"
              data-aos="fade-right"
          >
            <h3 class="text-white font-bold text-[45px]">
              {{ index.name }}
            </h3>
            <div class="w-3/4">
              <p class="whitespace-normal">{{ index.description }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { onMounted } from 'vue';
import AOS from 'aos';
import 'aos/dist/aos.css';

const services = [
  {
    id: 1,
    name: "Web Development",
    description: "We develop websites with the high quality, from corporate websites to web applications",
  },
  {
    id: 2,
    name: "Mobile Apps",
    description: "Developing a project MindMap and designing it with the optimal solution based on its architecture",
  },
  {
    id: 3,
    name: "Ui&UX",
    description: "We develop websites with the high quality, from corporate websites to web applications",
  },
  {
    id: 4,
    name: "Media Production",
    description: "Developing a project MindMap and designing it with the optimal solution based on its architecture",
  },
  {
    id: 5,
    name: "CRM System",
    description: "Developing a project MindMap and designing it with the optimal solution based on its architecture",
  },
  {
    id: 6,
    name: "Branding",
    description: "Automation of business and processes, development of electronic management systems that reduce paper-work by 100%",
  },
  {
    id: 7,
    name: "Production of games",
    description: "Developing a creative and unique logo for your project and create its branding guidelines"
  },
  {
    id: 8,
    name: "Artificial intelligence",
    description: "Development of games of any subject and complexity, corresponding to the international level."
  },
  {
    id: 9,
    name: "Cybersecurity",
    description: "We develop websites with the high quality, from corporate websites to web applications"
  },
];

onMounted(() => {
  AOS.init({
    duration: 1000, // Duration of the animation
    easing: 'ease-in-out', // Easing function
    once: true, // Whether animation should happen only once
  });
});


</script>

<style lang="scss" scoped>
.container{
  max-width: 1310px;
}
</style>
