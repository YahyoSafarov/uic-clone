<template>
  <div class="container">
    <div>
      <div data-aos="fade-up-left">
        <h2 class="text-white text-[25px] font-bold">
          UIC Clan
        </h2>
        <p class="text-white text-[15px] font-medium">
          The eSports CS:GO team UIC Clan deserve special attention, because Players, they are employees, show impressive results in major tournaments among other professional players. The team was honored to participate in such a CAD Corporate Cup tournament, by clicking on the
           <span class="text-[#00A795]"><NuxtLink to="https://www.youtube.com/watch?v=mFybAaWBwqo" target="_blank">link</NuxtLink></span> you can see the game of our team in the tournament, where it was noted as one of the most ambitious teams and showed impressive results.
        </p>
      </div>

        <div class="relative bg-[#252527] flex flex-col gap-10 mt-44 border-[#37373A] border-[2px] rounded-[24px] p-10">
          <div class="mb-14">
            <img src="https://uic.group/uic-images/about/uic-clan.png" class="absolute top-0 left-[50%] translate-x-[-50%] translate-y-[-50%] w-[140px] h-[140px]" alt="no image">
          </div>
          <div class="flex items-center justify-center gap-10" data-aos="fade-up-left">
            <div class="border-[transparent] border-[1px] rounded-[10px] duration-300 hover:border-[#00A795] hover:translate-y-[-5px] cursor-pointer aos-init aos-animate">
              <img src="https://uic.group/uic-images/image/uic_clan1.png" alt="no image">
            </div>
            <div class="border-[transparent] border-[1px] rounded-[10px] duration-300 hover:border-[#00A795] hover:translate-y-[-5px] cursor-pointer aos-init aos-animate">
              <img src="https://uic.group/uic-images/image/uic_clan2.png" alt="no image">
            </div>
          </div>
          <div class="flex items-center justify-center gap-10" data-aos="fade-up-left">
            <div class="border-[transparent] border-[1px] rounded-[10px] duration-300 hover:border-[#00A795] hover:translate-y-[-5px] cursor-pointer aos-init aos-animate">
              <img src="https://uic.group/uic-images/image/uic_clan3.png" alt="no image">
            </div>
            <div class="border-[transparent] border-[1px] rounded-[10px] duration-300 hover:border-[#00A795] hover:translate-y-[-5px] cursor-pointer aos-init aos-animate">
              <img src="https://uic.group/uic-images/image/uic_clan4.png" alt="no image">
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

const image = [
  {
    id: 1,
    src: "\thttps://uic.group/uic-images/image/uic_clan1.png",
  },
  {
    id: 2,
    src: "\thttps://uic.group/uic-images/image/uic_clan2.png",
  },
  {
    id: 3,
    src: "https://uic.group/uic-images/image/uic_clan3.png",
  },
  {
    id: 4,
    src: "https://uic.group/uic-images/image/uic_clan4.png",
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

.grid_img{
  display: flex;
  flex-direction: column;
}
</style>