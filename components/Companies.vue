<template>
  <div class="bg-black">
    <div class="container py-36">
      <div data-aos="fade-up">
        <div data-aos="fade-left">
          <p class="text-[#00a795] font-bold">OUR PARTNERS</p>
          <h2 class="text-white font-bold text-[35px] mb-24">Companies that believe in us</h2>
        </div>

      </div>

      <div class="">
        <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-5 gap-10 media_grid" data-aos="fade-up">
          <NuxtLink v-for="item in images" :key="item" :href="item.href" data-aos="fade-left" target="_blank"
                    class=" bg-[#141415] p-4 rounded-[10px]"
          >
            <img :src="item.srs" class="w-full h-[150px] duration-300 grayscale hover:grayscale-0" alt="no image">
          </NuxtLink>

        </div>
      </div>
    </div>
  </div>

</template>

<script setup>

import { onMounted } from "vue";
import AOS from 'aos';
import 'aos/dist/aos.css'

const images = [
  {
    id: 1,
    srs: "https://uic.group/media/Partners/Asakabank.svg",
    href: "https://www.asakabank.uz/",
  },

  {
    id: 2,
    srs: "https://uic.group/media/Partners/Avloniy.svg",
    href: "https://avloniy.uz/",
  },
  {
    id: 3,
    srs: "https://uic.group/media/Partners/Az_Capital_1.png",
    href: "https://azcapital.uz/",
  },
  {
    id: 4,
    srs: "https://uic.group/media/Partners/Express_24.svg",
    href: "https://express24.uz/",
  },
  {
    id: 5,
    srs: "https://uic.group/media/Partners/IT_park.svg",
    href: "https://it-park.uz/",
  },
  {
    id: 6,
    srs: "https://uic.group/media/Partners/milliy-gvardiya_copy_copy.svg",
    href: "https://www.milliygvardiya.uz/",
  },
  {
    id: 7,
    srs: "https://uic.group/media/Partners/Mininovvation.svg",
    href: "https://mininnovation.uz/",
  },
  {
    id: 8,
    srs: "https://uic.group/media/Partners/PM.svg",
    href: "https://projectmanagers.uz/",
  },
  {
    id: 9,
    srs: "https://uic.group/media/Partners/Pro_SM.svg",
    href: "https://prosm.uz/",
  },
  {
    id: 10,
    srs: "https://uic.group/media/Partners/TDIU.svg",
    href: "https://tsue.uz/en",
  },
  {
    id: 11,
    srs: "https://uic.group/media/Partners/Uzcard.svg",
    href: "https://www.uzcard.uz/uz",
  },
  {
    id: 12,
    srs: "https://uic.group/media/Partners/Group_18791.svg",
    href: "https://yoshlar.gov.uz/uz/",
  },
  {
    id: 13,
    srs: "https://uic.group/media/Partners/YOSHLAR_ITTIFOQI-01%D1%86%D1%83%D0%B0%D0%BF%D0%B2%D1%8B%D0%BF.png",
    href: "https://yoshlarittifoqi.uz/",
  },
  {
    id: 14,
    srs: "https://uic.group/media/Partners/TMCI_eaFjgNO.svg",
    href: "https://tmci.uz/",
  },
  {
    id: 15,
    srs: "https://uic.group/media/Partners/CSC_logo_light_JjM0jSn.svg",
    href: "https://csec.uz/ru/",
  },
  {
    id: 16,
    srs: "https://uic.group/media/Partners/Dark_H_Moto_-removebg.png",
    href: "https://cyberpark.uz/?lang=en",
  },
  {
    id: 17,
    srs: "https://uic.group/media/Partners/uzclub.svg",
    href: "https://uzbekistans.club/",
  },
  {
    id: 18,
    srs: "https://uic.group/media/Partners/zor_tv_colored.svg",
    href: "https://zortv.uz/",
  },
  {
    id: 19,
    srs: "https://uic.group/media/Partners/SELLO.svg",
    href: "https://sello.uz/uz",
  },
  {
    id: 20,
    srs: "https://uic.group/media/Partners/paylov_color.svg",
    href: "https://paylov.uz/",
  },
  {
    id: 21,
    srs: "https://uic.group/media/Partners/ipotekabank_XVMESno.svg",
    href: "https://www.ipotekabank.uz/",
  },
]


onMounted( () => {
  AOS.init ({
    duration: 1000,
    easing: 'ease-in-out',
    once: true,
  })
})
</script>

<style lang="scss" scoped>

</style>