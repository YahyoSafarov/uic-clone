<template>
  <div class="container py-36">
    <div class="bg-[#252525] p-20 w-full rounded-[12px]" data-aos="fade-up">
      <div class="flex gap-[20rem] items-center place-items-center"  data-aos-anchor-placement="center-bottom">
        <div>
          <h2 class="text-white font-bold text-[45px]">
            You can also be among this <br> team :)
          </h2>
          <p>
            Do you want to growth with us? Now prove to us that you need it! Become an integral <br> part of the team
          </p>
        </div>

        <div class="flex cursor-pointer  flex-col gap-6">
          <div class="flex items-center gap-6">
            <div class="border-t-[2px] border-[#999999] w-[30px]"></div>
            <h2 class="text-[#fff] font-bold text-[16px] duration-300 hover:text-[#00a795]">Flutter developer</h2>
          </div>

          <div class="flex items-center gap-6 ">
            <div class="border-t-[2px] border-[#999999] w-[30px]"></div>
            <h2 class="text-[#fff] font-bold text-[16px] duration-300 hover:text-[#00a795]">UI?UX designer</h2>
          </div>

          <div class="flex items-center gap-6 ">
            <div class="border-t-[2px] border-[#999999] w-[30px]"></div>
            <h2 class="text-[#fff] font-bold text-[16px] duration-300 hover:text-[#00a795]">AI Engineer</h2>
          </div>

          <div class="flex items-center gap-6 ">
            <div class="border-t-[2px] border-[#999999] w-[30px]"></div>
            <h2 class="text-[#fff] font-bold text-[16px] duration-300 hover:text-[#00a795]">HR maneger</h2>
          </div>

        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { onMounted } from "vue";
import AOS from 'aos';
import 'aos/dist/aos.css'


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