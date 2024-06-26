<template>
  <div class="container py-14">
    <div>
      <h3 class="text-white font-bold text-[25px] mb-8" data-aos="fade-left">
        Currently, our company offers its IT solutions in 9 main areas:
      </h3>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-3 gap-10">
      <div v-for="item in services" :key="item"
      >
        <NuxtLink to="">
          <div class="bg-[#252527] md:px-6 p-2 md:p-5 rounded-[12px] lg:min-h-[180px] border-[transparent] border-[2px] border-solid transition-all duration-300 hover:border-[#00A795]" data-aos="zoom-in-left">
            <h2 class="text-[13px] md:text-[16px] lg:text-[24px] font-bold leading-[120%] mb-3 text-white">{{item.name}}</h2>
            <p class="text-[#E0E0E099] text-[12px] md:text-[14px] lg:text-[16px] leading-[140%]">{{item.description}}</p>
          </div>
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script setup>
import {onMounted} from "vue";
import AOS from 'aos';
import 'aos/dist/aos.css'

const services = [
  {
    id: 1,
    name: "Web Development",
    description: "We develop websites with the high quality, from corporate websites to web applications",
  },
  {
    id: 2,
    name: "UI&UX",
    description: "Developing a project MindMap and designing it with the optimal solution based on its architecture",
  },
  {
    id: 3,
    name: "CRM Systems",
    description: "Automation of business and processes, development of electronic management systems that reduce paper-work by 100%",
  },
  {
    id: 4,
    name: "Mobile apps",
    description: "Development and technical support of mobile applications of any complexity",
  },
  {
    id: 8,
    name: "Media production",
    description: "Professional preparation of 2D / 3D animation, project presentation, advertising, video and other media resources.",
  },
  {
    id: 6,
    name: "Branding",
    description: "Developing a creative and unique logo for your project and create its branding guidelines",
  },
  {
    id: 7,
    name: "Cybersecurity",
    description: "Find and fix vulnerabilities in networks, devices, code, and data.",
  },
  {
    id: 8,
    name: "Production of games",
    description: "Development of games of any subject and complexity, corresponding to the international level.",
  },
  {
    id: 9,
    name: "Artificial intelligence",
    description: "Development of intelligent computer systems with the capabilities of human intelligence.",
  },
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
</style>