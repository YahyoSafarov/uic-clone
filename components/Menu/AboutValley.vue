<template>
  <div class="container">
    <div class="border-neutral-700 bg-[#252527] rounded-[16px]"
         data-aos="fade-left"
    >
      <div class="grid grid-cols-2 gap-4">
       <div class="p-10">
         <h2 class="text-white font-bold text-[25px]">We are in Silicon Valley</h2>
         <p data-v-b76aee44="" class="text-[14px] text-white md:text-[16px] leading-[140%] font-medium mb-32 sm:mb-10">In order to further develop the company, enter the international arena and improve the professional skills of team members, a branch of the company was opened <span data-v-b76aee44="" class="text-[#00A795]">in San Francisco (Silicon Valley) in California</span> , USA.</p>
       </div>
        <div class="overflow-hidden">
          <img src="https://cdn.commeta.uz/562x279/https://cdn.commeta.uz/media/uploaded/2023/10/12/1616653640968.jpeg" class="w-[550px] h-[348px] object-cover rounded-[16px] fiter_img absolute" alt="no image">
        </div>
      </div>

      <div class="p-10 relative z-50">
        <p data-v-b76aee44="" class="max-w-[820px] text-[#FFFFFF80] leading-[144%] text-[14px] md:text-[16px]">This solution will serve as an excellent tool for improving the skills of employees who want to get an education. <span data-v-b76aee44="" class="text-[#fff]">Special grants from the company </span> will be allocated.</p>
      </div>
    </div>
  </div>
</template>

<script setup>
import {onMounted} from "vue";
import AOS from 'aos';
import 'aos/dist/aos.css'

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

.fiter_img{
  filter: brightness(20%);
}
</style>