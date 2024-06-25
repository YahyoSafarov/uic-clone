<template>
  <div class="container h-[600px]">
    <swiper
        :scrollbar="{
      hide: true,
      color: '#00a795',
    }"
        :modules="modules"
        class="mySwiper"
    >
      <swiper-slide>
        <div class="grid grid-cols-2">
          <div class="flex flex-col gap-20">
            <div class="flex items-center gap-[4rem]">
              <img src="https://uic.group/media/AboutUs/_A8A1925_HQCUw7a.jpeg" class="w-[60px] rounded-full" alt="no image">
              <div>
                <h3 class="text-white font-bold text-[18px]">Sharipov Kongratboy</h3>
                <p>Rector of Tashkent State University of Economics</p>
              </div>
            </div>
            <div>
              <i data-v-56c03d90="" data-v-643a1fb5="" class="icon hover:text-red-500 md:w-[48px] w-[32px] md:h-[48px] h-[32px] text-[#00A795]"><svg width="48" height="48" viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M11.6025 40.8001C17.445 40.8001 22.005 36.2401 22.005 30.5401C22.005 24.6976 17.445 20.1376 11.6025 20.1376C11.6025 16.1476 12.7425 11.8726 14.4525 8.16759C14.88 7.3126 14.4525 6.6001 13.455 6.6001H11.6025C11.0325 6.6001 10.605 6.7426 10.035 7.3126C6.61495 11.1601 1.19995 19.5676 1.19995 29.1151C1.19995 36.2401 5.90245 40.8001 11.6025 40.8001ZM36.9675 40.8001C42.81 40.8001 47.37 36.2401 47.37 30.5401C47.37 24.6976 42.81 20.1376 36.9675 20.1376C36.9675 16.1476 38.1075 11.8726 39.8175 8.16759C40.245 7.3126 39.8175 6.6001 38.82 6.6001H36.9675C36.3975 6.6001 35.97 6.7426 35.4 7.3126C31.98 11.1601 26.565 19.5676 26.565 29.1151C26.565 36.2401 31.2675 40.8001 36.9675 40.8001Z" fill="#00A795"></path>
              </svg>
              </i>

              <div class="mt-5">
                <p class="text-white font-bold text-[20px]">TDIU reestrlik tizimining  samarali yo’lga qo’yilishi</p>
              </div>

              <div class="flex gap-10 mt-10 items-center
">
                <p class="text-gray-400 text-[15px]">Personnel registry system</p>
                <NuxtLink to="https://argos.uz/oz" class="text-[#00a795] font-bold cursor-pointer">WEBSITE</NuxtLink>
              </div>
            </div>
          </div>


          <div>
            Toshkent Davlat iqtisodiyot universiteti kadrlar reestrlik tizimini “UIC&nbsp; Group” jamoasi bilan birgalikda yo’lga qo’ydi. Bu optimallashtirish kadrlar boshqaruv tizimini yanada osonlashtirdi. TDIU jamoasi &nbsp;“UIC Group” IT kompaniyasining malakali mutaxassislariga o'z minnatdorchiligini bildiradi.
          </div>
        </div>

      </swiper-slide>
      <swiper-slide>
        <div class="grid grid-cols-2">
          <div class="flex flex-col gap-20">
            <div class="flex items-center gap-[4rem]">
              <img src="https://uic.group/media/AboutUs/_A8A1925_HQCUw7a.jpeg" class="w-[60px] rounded-full" alt="no image">
              <div>
                <h3 class="text-white font-bold text-[18px]">Sharipov Kongratboy</h3>
                <p>Rector of Tashkent State University of Economics</p>
              </div>
            </div>
            <div>
              <i data-v-56c03d90="" data-v-643a1fb5="" class="icon hover:text-red-500 md:w-[48px] w-[32px] md:h-[48px] h-[32px] text-[#00A795]"><svg width="48" height="48" viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M11.6025 40.8001C17.445 40.8001 22.005 36.2401 22.005 30.5401C22.005 24.6976 17.445 20.1376 11.6025 20.1376C11.6025 16.1476 12.7425 11.8726 14.4525 8.16759C14.88 7.3126 14.4525 6.6001 13.455 6.6001H11.6025C11.0325 6.6001 10.605 6.7426 10.035 7.3126C6.61495 11.1601 1.19995 19.5676 1.19995 29.1151C1.19995 36.2401 5.90245 40.8001 11.6025 40.8001ZM36.9675 40.8001C42.81 40.8001 47.37 36.2401 47.37 30.5401C47.37 24.6976 42.81 20.1376 36.9675 20.1376C36.9675 16.1476 38.1075 11.8726 39.8175 8.16759C40.245 7.3126 39.8175 6.6001 38.82 6.6001H36.9675C36.3975 6.6001 35.97 6.7426 35.4 7.3126C31.98 11.1601 26.565 19.5676 26.565 29.1151C26.565 36.2401 31.2675 40.8001 36.9675 40.8001Z" fill="#00A795"></path>
              </svg>
              </i>

              <div class="mt-5">
                <p class="text-white font-bold text-[20px]">TDIU reestrlik tizimining  samarali yo’lga qo’yilishi</p>
              </div>

              <div class="flex gap-10 mt-10 items-center
">
                <p class="text-gray-400 text-[15px]">Personnel registry system</p>
                <NuxtLink to="https://argos.uz/oz" class="text-[#00a795] font-bold cursor-pointer">WEBSITE</NuxtLink>
              </div>
            </div>
          </div>


          <div>
            Toshkent Davlat iqtisodiyot universiteti kadrlar reestrlik tizimini “UIC&nbsp; Group” jamoasi bilan birgalikda yo’lga qo’ydi. Bu optimallashtirish kadrlar boshqaruv tizimini yanada osonlashtirdi. TDIU jamoasi &nbsp;“UIC Group” IT kompaniyasining malakali mutaxassislariga o'z minnatdorchiligini bildiradi.
          </div>
        </div>

      </swiper-slide>
      <swiper-slide>
        <div class="grid grid-cols-2">
          <div class="flex flex-col gap-20">
            <div class="flex items-center gap-[4rem]">
              <img src="https://uic.group/media/AboutUs/_A8A1925_HQCUw7a.jpeg" class="w-[60px] rounded-full" alt="no image">
              <div>
                <h3 class="text-white font-bold text-[18px]">Sharipov Kongratboy</h3>
                <p>Rector of Tashkent State University of Economics</p>
              </div>
            </div>
            <div>
              <i data-v-56c03d90="" data-v-643a1fb5="" class="icon hover:text-red-500 md:w-[48px] w-[32px] md:h-[48px] h-[32px] text-[#00A795]"><svg width="48" height="48" viewBox="0 0 48 48" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M11.6025 40.8001C17.445 40.8001 22.005 36.2401 22.005 30.5401C22.005 24.6976 17.445 20.1376 11.6025 20.1376C11.6025 16.1476 12.7425 11.8726 14.4525 8.16759C14.88 7.3126 14.4525 6.6001 13.455 6.6001H11.6025C11.0325 6.6001 10.605 6.7426 10.035 7.3126C6.61495 11.1601 1.19995 19.5676 1.19995 29.1151C1.19995 36.2401 5.90245 40.8001 11.6025 40.8001ZM36.9675 40.8001C42.81 40.8001 47.37 36.2401 47.37 30.5401C47.37 24.6976 42.81 20.1376 36.9675 20.1376C36.9675 16.1476 38.1075 11.8726 39.8175 8.16759C40.245 7.3126 39.8175 6.6001 38.82 6.6001H36.9675C36.3975 6.6001 35.97 6.7426 35.4 7.3126C31.98 11.1601 26.565 19.5676 26.565 29.1151C26.565 36.2401 31.2675 40.8001 36.9675 40.8001Z" fill="#00A795"></path>
              </svg>
              </i>

              <div class="mt-5">
                <p class="text-white font-bold text-[20px]">TDIU reestrlik tizimining  samarali yo’lga qo’yilishi</p>
              </div>

              <div class="flex gap-10 mt-10 items-center
">
                <p class="text-gray-400 text-[15px]">Personnel registry system</p>
                <NuxtLink to="https://argos.uz/oz" class="text-[#00a795] font-bold cursor-pointer">WEBSITE</NuxtLink>
              </div>
            </div>
          </div>


          <div>
            Toshkent Davlat iqtisodiyot universiteti kadrlar reestrlik tizimini “UIC&nbsp; Group” jamoasi bilan birgalikda yo’lga qo’ydi. Bu optimallashtirish kadrlar boshqaruv tizimini yanada osonlashtirdi. TDIU jamoasi &nbsp;“UIC Group” IT kompaniyasining malakali mutaxassislariga o'z minnatdorchiligini bildiradi.
          </div>
        </div>

      </swiper-slide>
    </swiper>
  </div>

</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import 'swiper/css/scrollbar';


// import required modules
import { Scrollbar } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Scrollbar],
    };
  },
};
</script>


<style lang="scss" scoped>
.container{
  max-width: 1320px;
}
.swiper {
  width: 100%;
  height: 100%;
}

.swiper-slide {

  /* Center slide text vertically */
  display: flex;
  justify-content: start;
  align-items: center;
}

.swiper-slide img {
  display: block;
  object-fit: cover;
}

</style>