<template>
  <div class="container">
    <div class="py-24">
      <div data-aos="fade-up"
           data-aos-anchor-placement="bottom-bottom">
        <h2 class="text-white text-[25px] font-bold py-12">
          Additional pluses:
        </h2>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-2 gap-7">
        <div v-for="item in cloud" :key="item"
        >
          <div class="bg-[#252527] flex items-center h-[120px] rounded-[12px] md:h-[80px] lg:h-[80px]"
               data-aos="fade-up-left"
          >
            <div class="border-l-4 border-[#00A795] h-[30px] flex items-center"
            >
              <div class="p-10">
                <p class="text-white text-[15px]">{{item.text}}</p>
              </div>
            </div>
          </div>
          <div class="border-l-2 border-red-900"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import {onMounted} from "vue";
import AOS from 'aos';
import 'aos/dist/aos.css'

const cloud = [
  {
    id: 1,
    text: "A licensed version of the Windows software",
  },
  {
    id: 2,
    text: "Licensed antivirus for each device",
  },
  {
    id: 3,
    text: "Monthly bonus system (in addition to the basic monthly salary, additional bonuses can be obtained through monthly initiatives in accordance with existing criteria)",
  },
  {
    id: 4,
    text: "Location in the city center (within walking distance from the Oybek metro station and bus stops, convenient parking, a minute from Korzinka.uz, pharmacies and cafes)",
  },
  {
    id: 5,
    text: "Comfortable office with all conditions",
  },
  {
    id: 6,
    text: "\n" +
        "The company's employees are allocated computers according to their needs",
  },
  {
    id: 7,
    text: "Opportunity to work in a large and friendly team",
  },
  {
    id: 8,
    text: "Training from experienced professionals",
  },
  {
    id: 9,
    text: "Work in large-scale projects (local and foreign projects)",
  },
  {
    id: 10,
    text: "Official employment (according to the labor code of the Republic of Uzbekistan)",
  },
  {
    id: 11,
    text: "Business trips (to regions and international countries)",
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