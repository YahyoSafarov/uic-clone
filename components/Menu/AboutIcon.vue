<template>
  <div class="container">
    <div>
      <div class="flex flex-col gap-10"
      >
        <div v-for="item in icon" :key="item.name" data-aos="fade-up"
        >
          <h2 class="text-white text-[25px] font-bold mb-4" data-aos-anchor-placement="bottom-bottom">
            {{item.name}}
          </h2>
          <div class="flex items-center gap-10" data-aos-anchor-placement="bottom-bottom">
            <i data-v-56c03d90="" class="icon hover:text-red-500"><svg width="44" height="44" viewBox="0 0 44 44" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M16.5 21.9999L20.1667 25.6666L27.5 18.3333" stroke="#00A795" stroke-width="2.8" stroke-linecap="round" stroke-linejoin="round"></path>
              <path d="M21.9999 5.5C26.2823 9.28872 31.8714 11.2614 37.5832 11C39.2634 16.7155 38.5538 22.868 35.6168 28.051C32.6798 33.234 27.7664 37.0043 21.9999 38.5C16.2334 37.0043 11.32 33.234 8.383 28.051C5.44597 22.868 4.73643 16.7155 6.41657 11C12.1284 11.2614 17.7176 9.28872 21.9999 5.5" stroke="#00A795" stroke-width="2.8" stroke-linecap="round" stroke-linejoin="round"></path>
            </svg>
            </i>
            <p class="text-white text-[17px]">{{item.desc}}</p>
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

const icon = [
  {
    id: 1,
    name: "The company offered solutions for the education system of the Republic of Uzbekistan in projects:",
    src: "",
    desc: "Co-Learning Academy is a social project for teaching IT professions. This project includes training in such areas as Advanced Front-end, Basic Front-end, Python Back-end, PHP Back-end, Graphic Design and Mobile Development. Training to take place on a phased study of video lessons directly from specialists."
  },
  {
    id: 2,
    src: "",
    desc: "Mental arithmetic - automated multifunctional platform! As a modern platform for teachers teaching in this field, we have created a homework system in the form of a website and mobile application for children, they are specially designed in the style of exciting games. The platform is currently among the largest startups in the B2B direction.",
  },
  {
    id: 3,
    src: "",
    desc: "iMaktab — aims to provide all schools, regardless of their size or the resources they have, with the systems they need to provide effective learning, teaching and school management. iMaktab is developed with Python, Django, VueJS, PostgreSQL and other software development tools.",
  },
  {
    id: 4,
    name: "In the field of state administration",
    src: "",
    desc: "Yosh saylovchi is an information website has been prepared to attract the attention of young voters and use their constitutional rights in the elections of the President of the Republic of Uzbekistan in 2021. On the site, visitors have the opportunity to see where polling stations are located by entering their data."
  },
  {
    id: 5,
    src: "",
    desc: "Meningkonstitutsiyam.uz is a web portal that allows expanding the opportunities for the participation of citizens of our country in the implementation of constitutional reforms, obtaining prompt and reliable information about the activities of the Constitutional Commission, familiarizing with the positions of representatives of the general public, specialists and experts on issues put forward for public discussion.",
  },
  {
    id: 6,
    src: "",
    desc: "The project of the Notary Chamber provides many opportunities by integrating all electronic services of the Notary Chamber of the Republic of Uzbekistan. The site serves to bring together all notary services across the country and make their information easily accessible to users.",
  },
  {
    id: 7,
    src: "",
    desc: "Sergelihokimiyati.uz - the official page of the district khokimiyat has been qualitatively enriched with the help of our services. The ability to manage vacancies from admin panels, a system for automatically generating resumes by applicants and a high-speed website - all this is dynamic and interactive on the khokimiyat website.",
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