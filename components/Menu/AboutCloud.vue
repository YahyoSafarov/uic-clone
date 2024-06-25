<template>
  <div class="container">
    <div class="py-24">
      <div data-aos="fade-up"
           data-aos-anchor-placement="bottom-bottom">
        <h2 class="text-white text-[25px] font-bold py-12">
          A cloud-based site management program - Wave, which has such functionality as:
        </h2>
      </div>

      <div class="grid grid-cols-3 gap-7">
        <div v-for="item in cloud" :key="item"
        >
          <div class="bg-[#252527] flex items-center h-[100px] rounded-[12px]"
               data-aos="fade-up-left"
          >
            <div class="border-l-4 border-[#555] h-[50px] flex items-center"
            >
              <div class="p-10">
                <p class="text-white text-[18px]">{{item.text}}</p>
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
    text: "Manage and edit site data",
  },
  {
    id: 2,
    text: "Adding, editing and deleting links to the site",
  },
  {
    id: 3,
    text: "Add pages to the site to edit and delete them",
  },
  {
    id: 4,
    text: "Ability to change the basic settings on the site",
  },
  {
    id: 5,
    text: "Enabling and disabling the main options on the site",
  },
  {
    id: 6,
    text: "Management of the SEO structure of the site",
  },
  {
    id: 7,
    text: "Management of sections of the site",
  },
  {
    id: 8,
    text: "Control system users",
  },
  {
    id: 9,
    text: "Manage media files (photo/video/audio)",
  },
  {
    id: 10,
    text: "Maintenance of site statistics",
  },
  {
    id: 11,
    text: "Management of advertising information on the site",
  },
  {
    id: 12,
    text: "Managing forms on the site and accepting applications",
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