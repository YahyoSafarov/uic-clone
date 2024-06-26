<template>
  <div class="container">
    <div class=" flex flex-col justify-center py-6 sm:py-12">
      <div class="p-6 container mx-auto">

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-10 items-center">

          <div v-for="index in item" :key="index.name" data-aos="fade-up"
          >
            <!-- blog article card -->
            <NuxtLink :to="`/vacancy/${item.id}`">
              <article data-aos="fade-right" class="p-10 h-[190px] w-[420px] m-5 bg-[#222222] transition duration-300 group transform hover:-translate-y-2 hover:shadow-2xl rounded-2xl cursor-pointer">
                <a href="#" class="absolute opacity-0 top-0 right-0 left-0 bottom-0"></a>
                <div class="relative mb-10 rounded-[22px]">
                  <h1 class="font-bold text-[20px] text-white">{{index.name}}</h1>
                  <div class="border-b-[2px] border-[#333] mt-10"></div>
                  <!--              <a class="flex justify-center items-center bg-purple-500 bg-opacity-80 z-10 absolute top-0 left-0 w-full h-full text-white rounded-2xl opacity-0 transition-all duration-300 transform group-hover:scale-105 text-xl group-hover:opacity-100" href="#" target="_blank" rel="noopener noreferrer">-->
                  <!--                Read article <svg class="ml-2 w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 5l7 7-7 7M5 5l7 7-7 7"></path></svg>-->
                  <!--              </a>-->

                </div>
                <!-- blog info -->


                <div class="flex items-center justify-between">
                  <div class="flex items-center gap-4">
                    <i data-v-56c03d90="" data-v-c9fd75cc="" class="icon hover:text-red-500"><svg width="12" height="14" viewBox="0 0 12 14" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path d="M0.861328 5.50245H11.1444" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                      <path d="M8.5629 7.75559H8.56824" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                      <path d="M6.00284 7.75559H6.00818" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                      <path d="M3.4379 7.75559H3.44324" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                      <path d="M8.5629 9.99781H8.56824" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                      <path d="M6.00284 9.99781H6.00818" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                      <path d="M3.4379 9.99781H3.44324" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                      <path d="M8.33315 1.23077V3.12929" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                      <path d="M3.67299 1.23077V3.12929" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                      <path fill-rule="evenodd" clip-rule="evenodd" d="M8.44557 2.14184H3.56058C1.86634 2.14184 0.808105 3.08565 0.808105 4.82051V10.0415C0.808105 11.8036 1.86634 12.7692 3.56058 12.7692H8.44022C10.1398 12.7692 11.1927 11.82 11.1927 10.0851V4.82051C11.198 3.08565 10.1452 2.14184 8.44557 2.14184Z" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                    </svg>
                    </i>
                    <h3 class="font-medium text-[15px] leading-8">
                      <a href="#" class="block relative group-hover:text-white transition-colors duration-200">
                        MONDAY-FRIDAY
                      </a>
                    </h3>
                  </div>

                  <div class="flex gap-4 items-center">
                    <i data-v-56c03d90="" data-v-c9fd75cc="" class="icon hover:text-red-500"><svg width="12" height="12" viewBox="0 0 12 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path fill-rule="evenodd" clip-rule="evenodd" d="M11.3367 6.00028C11.3367 8.94778 8.94761 11.3368 6.00011 11.3368C3.05261 11.3368 0.663574 8.94778 0.663574 6.00028C0.663574 3.05278 3.05261 0.663742 6.00011 0.663742C8.94761 0.663742 11.3367 3.05278 11.3367 6.00028Z" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                      <path d="M7.97969 7.69782L5.80469 6.40032V3.60397" stroke="white" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
                    </svg>
                    </i>

                    <h3 class="font-medium text-[15px] leading-8">
                      <a href="#" class="block relative group-hover:text-white transition-colors duration-200">
                        09:00-18:00
                      </a>
                    </h3>
                  </div>
                </div>
                <div class="">
                  <div class=" mt-16 border-neutral-700 gap-4 bg-[#111] ml-1
               items-center justify-between flex duration-300 p-3 rounded-2xl group-hover:bg-[#00a795]">
                    <i data-v-56c03d90="" data-v-c9fd75cc="" class="icon hover:text-red-500 text-[#00A795] group-hover:text-white transition-colors"><svg width="22" height="22" viewBox="0 0 22 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path d="M3.26586 19.6625C3.28304 19.8344 3.38617 19.9719 3.52367 20.0578C3.60961 20.0922 3.69555 20.1266 3.78148 20.1266C3.85023 20.1266 3.93617 20.1094 4.00492 20.075L5.25961 19.4734C9.09242 17.6344 13.3549 16.6719 17.6174 16.6719H19.9377C20.2299 16.6719 20.4534 16.4484 20.4534 16.1562C20.4534 15.8641 20.2299 15.6406 19.9377 15.6406H17.6174C13.2174 15.6406 8.80023 16.6375 4.81273 18.5281L4.21117 18.8203L3.95336 16.6031C3.91898 16.3281 3.66117 16.1219 3.38617 16.1562C3.11117 16.1906 2.90492 16.4484 2.9393 16.7234L3.26586 19.6625Z" fill="#00A795"></path>
                      <path d="M1.71875 8.9375C2.01094 8.9375 2.23438 8.71406 2.23438 8.42188C2.23438 8.12969 2.01094 7.90625 1.71875 7.90625C1.42656 7.90625 1.20312 7.68281 1.20312 7.39062C1.20312 7.09844 1.42656 6.875 1.71875 6.875H20.2812C20.5734 6.875 20.7969 7.09844 20.7969 7.39062C20.7969 7.68281 20.5734 7.90625 20.2812 7.90625C19.9891 7.90625 19.7656 8.12969 19.7656 8.42188C19.7656 8.71406 19.9891 8.9375 20.2812 8.9375C21.1406 8.9375 21.8281 8.25 21.8281 7.39062C21.8281 6.53125 21.1406 5.84375 20.2812 5.84375H1.71875C0.859375 5.84375 0.171875 6.53125 0.171875 7.39062C0.171875 8.25 0.859375 8.9375 1.71875 8.9375Z" fill="#00A795"></path>
                      <path d="M20.3497 14.7469C20.4528 14.6094 20.47 14.4547 20.4356 14.3L18.7169 8.28438C18.6481 8.06094 18.459 7.90625 18.2184 7.90625H3.78092C3.55748 7.90625 3.35123 8.06094 3.28248 8.28438L1.56373 14.3C1.51217 14.4547 1.54654 14.6266 1.64967 14.7469C1.75279 14.8844 1.90748 14.9531 2.06217 14.9531H19.9372C20.0919 14.9531 20.2465 14.8844 20.3497 14.7469ZM10.9997 12.0312C9.86529 12.0312 8.93717 11.3438 8.93717 10.4844C8.93717 9.625 9.86529 8.9375 10.9997 8.9375C12.134 8.9375 13.0622 9.625 13.0622 10.4844C13.0622 11.3438 12.134 12.0312 10.9997 12.0312Z" fill="#00A795"></path>
                    </svg>
                    </i>
                    <a class="block relative group-hover:text-white transition-colors duration-200 text-[18px]">
                      {{index.money}}
                    </a>
                    <button data-v-c9fd75cc="" class="bg-[#00A795] group-hover:bg-[#FFFFFF47] transition-colors h-[24px] w-[24px] rounded-full flex items-center justify-center" aria-label="button"><i data-v-56c03d90="" data-v-c9fd75cc="" class="icon hover:text-red-500"><svg width="16" height="12" viewBox="0 0 16 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path d="M9.05572 11L14.3335 6L1.00016 6M9.05572 1L14.3335 6L9.05572 1Z" stroke="#fff" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"></path>
                    </svg>
                    </i></button>
                  </div>
                </div>
              </article>
            </NuxtLink>

          </div>
        </div>


      </div>
    </div>
  </div>
</template>

<script setup>
import { onMounted } from 'vue';
import AOS from 'aos';
import 'aos/dist/aos.css';
const item = [
  {
    id: 1,
    name: "Flutter developer",
    money: "10 000 000 - 20 000 000 UZS",
    desccription: "FLutter developer",
  },
  {
    id: 2,
    name: "UI/UX designer",
    money: "10 000 000 - 15 000 000 UZS ",
    desccription: "Ui ux dewfef ",
  },
  {
    id: 3,
    name: "AI Engineer",
    money: "5 000 000 - 25 000 000 UZS",
  },
  {
    id: 4,
    name: "HR manager",
    money: "10 000 000 - 20 000 000 UZS",
  },
  {
    id: 5,
    name: "Project manager",
    money: "8 000 000 - 14 000 000 UZS",
  },
  {
    id: 6,
    name: "Frontend developer (VueJS)",
    money: "10 000 000 - 20 000 000 UZS",
  },
  {
    id: 7,
    name: "Sales Manager",
    money: "10 000 000 - 20 000 000 UZS",
  },
  {
    id: 8,
    name: "Backend developer (Odoo framework)",
    money: "10 000 000 - 25 000 000 UZS",
  },
  {
    id: 9,
    name: "Frontend developer (React.js)",
    money: "10 000 000 - 20 000 000 UZS",
  },
  {
    id: 10,
    name: "QA Engineer",
    money: "10 000 000 - 20 000 000 UZS",
  },
  {
    id: 11,
    name: "Backend developer (Python)",
    money: "10 000 000 - 20 000 000 UZS",
  },
  {
    id: 12,
    name: "Accountant",
    money: "8 000 000 - 10 000 000 UZS",
  },
]

onMounted(() => {
  AOS.init({
    duration: 1000, // Duration of the animation
    easing: 'ease-in-out', // Easing function
    once: true, // Whether animation should happen only once
  });
});
</script>

<style lang="scss" scoped>
article{
  will-change: transform; /*property in CSS optimizes animations*/
}
</style>