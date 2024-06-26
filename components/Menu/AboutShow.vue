<template>
  <div class="container md:py-24 lg:py-10">
    <div class="show-box bg-[#252527] duration-300 border-[#00A795] hover border-dashed rounded-[12px] border-[1px] p-6 flex items-center justify-center flex-col md:flex-row gap-y-8 mt-10 cursor-pointer" data-aos="fade-up">
      <div class="md:flex lg:flex justify-center items-center gap-14">
        <img src="https://media.licdn.com/dms/image/D4D22AQGucQuW8P2eFA/feedshare-shrink_800/0/1715782673317?e=2147483647&v=beta&t=4ykpL4WJuAc-pkXZzENfeXz4IXIyQGyz3xRunw6vFek"
             class="w-full max-w-[120px]"
             alt="image">
        <p class="text-white font-bold">You can find out more about our work in the showreel</p>

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

//
//.show-box:hover{
//  filter: drop-shadow(4px 4px 8px  #78dfbb);
//}
</style>