<template>
  <div class="container">
    <div class="py-24">
      <div data-aos="zoom-in-right">
        <h3 class="text-white font-bold text-[25px] mb-10">
          At the moment, the company employs more than 100 employees, in such areas as:
        </h3>
      </div>
      <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
        <div v-for="item in text" :href="item.href" :key="item"
        >
          <div class="flex border-[1px] border-[#FFFFFF33] group hover:bg-[#242426] rounded-[12px] cursor-pointer"
               data-aos="zoom-in-right"
          >
            <NuxtLink to="/career">
              <div class="flex gap-4 p-7">
                <span class=" font-bold group-hover:text-[#00A795] duration-300">#</span>
                <h1 class=" font-bold group-hover:text-[#fff] duration-300">{{item.title}}</h1>
              </div>
            </NuxtLink>
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
    title: "Front-end (Vue3)",
    href: "/career"
  },
  {
    id: 2,
    title: "Back-end (Python)",
    href: "/career"
  },
  {
    id: 3,
    title: "UX/UI",
    href: "/career"
  },
  {
    id: 4,
    title: "MA'LUMOTLAR TAHLILI",
    href: "/career"
  },
  {
    id: 5,
    title: "DevOps muhandisi",
    href: "/career"
  },
  {
    id: 6,
    title: "Mobil Devs (Flutter)",
    href: "/career"
  },
  {
    id: 7,
    title: "O'yin ishlab chiqaruvchilari",
    href: "/career"
  },
  {
    id: 8,
    title: "Loyiha menejerlari",
    href: "/career"
  },
  {
    id: 9,
    title: "Marketing menejerlari",
    href: "/career"
  },
  {
    id: 10,
    title: "QA muhandislari",
    href: "/career"
  },
  {
    id: 11,
    title: "Kontent menejeri",
    href: "/career"
  },
  {
    id: 12,
    title: "3D dizaynerlar",
    href: "/career"
  },
  {
    id: 13,
    title: "Koloristlar",
    href: "/career"
  },
  {
    id: 14,
    title: "Video muharrirlari",
    href: "/career"
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