<template>
  <div class="container">
    <div class="py-24">
      <div class="bg_color rounded-[24px]" data-aos="fade-up"
           data-aos-anchor-placement="bottom-bottom"
      >
        <div class="">
          <div class="overflow-hidden rounded-[12px]">
            <div class="">
              <div class="flex gap-10 media_flex">
                <img src="https://uic.group/uic-images/image/brend_year.png" class="rounded-l-[24px] rounded-r-[24px] sm:rounded-r-[0px] w-[100%] sm:w-[80%] md:w-[283px]" alt="no sertifecat">
                <div class="flex flex-col p-10">
                  <p class="text-white text-[20px] font-bold mb-10">
                    At the end of 2021, the company took 3rd place in the annual <span class="text-[#00A795] font-bold">“Year brand”</span> competition in the IT direction.
                  </p>
                  <div data-v-76870866="" class="flex items-start md:items-center flex-col md:flex-row gap-y-2 md:w-fit border-[#FFFFFF33] border-solid md:border-[1px] rounded-[12px] p-[6px] pl-2"><div data-v-76870866="" class="flex items-center gap-2"><i data-v-56c03d90="" data-v-76870866="" class="icon hover:text-red-500"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M11.1153 13.2131C10.2704 14.0142 10.348 15.3825 11.278 16.083L14.1722 18.2632C15.2583 19.0813 16.827 18.5135 17.1378 17.1897L19.5898 6.74707C19.7633 6.00821 19.0359 5.37834 18.3295 5.6556L4.42637 11.1119C3.60609 11.4338 3.63821 12.6055 4.4749 12.882L7.04049 13.7298C7.31606 13.8209 7.61823 13.7797 7.85942 13.6183L17.4732 7.18447L11.1153 13.2131Z" fill="white" fill-opacity="0.6"></path>
                  </svg>
                  </i><p data-v-76870866="" class="leading-[19px] tracking-[0.03em] text-[14px] md:text-[16px]"> https://t.me/uicgroup/247 </p></div><NuxtLink data-v-76870866="" href="https://t.me/uicgroup/247" target="_blank" class="bg-[#00A795] rounded-[6px] text-white text-[16px] py-1 px-8 md:px-2 md:ml-8 hover:bg-[#049282] duration-300">O'tish</NuxtLink>
                  </div>
                </div>
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
.bg_color{
  background-image: linear-gradient(150deg, rgba(0,0,0,0.2), rgba(0, 255, 225, 0.1));
}

@media(max-width: 690px){
  .media_flex{
    display: flex !important;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
}
</style>