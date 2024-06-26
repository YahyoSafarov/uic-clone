<template>
  <div class="container py-7">
    <div class="bg-[#252527] p-14 rounded-[12px]" data-aos="fade-up">
      <div>
        <p class="text-white text-[17px]">
          "UIC Group" is the address of projects that have their own values and do not pass without quality control. Every opportunity and demand in our company serves to meet the needs of our customers with maximum efficiency. Our company is ready to serve customers not just as customers, but as partners for life with the best offers!
        </p>
      </div>

      <div class=" flex flex-col gap-10 items-center justify-center py-10">
        <div v-for="index in item" :key="index" data-aos="fade-up" data-aos-anchor-placement="bottom-bottom" class=""
        >
          <div class="flex gap-14 items-center mediaflex">
              <img :src="index.image" class="min-w-[90px] flex-center" alt="no image">
              <p class="text-white mb-5">{{index.description}}</p>
          </div>
          <div class="none_media">
            <div class="border-b border-neutral-700 w-[920px] flex items-center justify-center ml-[122px]"></div>
          </div>
        </div>
      </div>
      <div class="wrapper flex justify-center items-center" data-aos="fade-up" data-aos-anchor-placement="bottom-bottom"
      >
        <NuxtLink to="/portfolio"> Portfolio</NuxtLink>
      </div>
    </div>

    <div class="py-14" data-aos="fade-up" data-aos-anchor-placement="bottom-bottom">
      <p class="text-white">
        The presence of our SaaS systems (these are the majority of services on the Internet: email, CRM systems, task schedulers, web designers for creating sites, blogging platforms. That is, all cloud programs that allow you to solve specific tasks) and PaaS (management system databases, machine learning environments or big data processing) in addition to core services.
      </p>
    </div>
  </div>
</template>

<script setup>
import {onMounted} from "vue";
import AOS from 'aos';
import 'aos/dist/aos.css'

const item = [
  {
    id: 1,
    image: "\thttps://uic.group/uic-images/about/portfolio/about-safenetpay.svg",
    description: "We have developed the safenetpay.com website of the international level using various types of animation that meet all cybersecurity requirements. Safenetpay is an international company engaged in the optimization of payment systems for companies.",
  },
  {
    id: 2,
    image: "https://uic.group/uic-images/about/portfolio/about-prosm.svg",
    description: "The “Pro Service Management” project, for this project our team gave a comprehensive solution - a mobile application, a website, a KPI system for employees, an automated billing system. The Pro SM project belongs to the Akfa holding group and manages all new buildings in Tashkent City. While our application provides services for all residents of new buildings.\n",
  },
  {
    id: 3,
    image: "https://uic.group/uic-images/about/portfolio/about-express24.svg",
    description: "A mobile application for the largest food delivery service Express24, as well as other solutions from our side. So Express 24 Merchant is a tool for establishments to receive orders and update order statuses and an application for managing a restaurant.",
  },
  {
    id: 4,
    image: "\thttps://uic.group/uic-images/about/portfolio/about-tdiu.svg",
    description: "Website for Tashkent State University of Economics with interactive features for staff, students and applicants of the university. Also, branding of the university, an HR system for automating work with personnel and mandatory testing of our products by a team of our QA engineers were carried out by our company.\n",
  },
  {
    id: 5,
    image: "\thttps://uic.group/uic-images/about/portfolio/about-vilz.svg",
    description: "For a company that sells cars of leading brands in Uzbekistan, I prepared the website Vilz.uz to increase sales of car dealerships. The site was prepared with the necessary options for registering for a test drive, buying a car on credit and other cars. The task was to create a mobile version of the site in the mode of a full-fledged online store and give the opportunity to read e-books. The mobile app is available on Google Play and the App Store.\n",
  },
  {
    id: 6,
    image: "https://uic.group/uic-images/about/portfolio/about-ayoluchun.svg",
    description: "Ayoluchun.uz, a special platform for women, provides them with comprehensive support, regardless of age and profession, and provides them with video lessons in areas of interest to them. Purpose: to unite women's education, spiritual, cultural and educational development on a single platform.\n",
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
//.wrapper{
//  position: fixed;
//  left: 50%;
//  transform: translate(-50%, -50%);
//}

a{
  display: block;
  width: 150px;
  line-height: 40px;
  background: transparent;
  text-align: center;
  position: relative;
  text-decoration: none;
  color: #fff;
  font-size: 15px;
  font-weight: 500;
  letter-spacing: 2px;
}

a:before,
a:after{
  position: absolute;
  content: "";
  transition: all .25s;
}

a:before{
  border-bottom: 2px solid #00a795;
  border-left: 2px solid #00a795;
  width: 10%;
  height: 33%;
  left: -10px;
  bottom: -10px;
}

a:after{
  border-top: 2px solid #00a795;
  border-right: 2px solid #00a795;
  width: 10%;
  height: 33%;
  top: -10px;
  right: -10px;
}

a:hover:before{
  width: 112%;
  height: 140%;
}

a:hover:after{
  width: 112%;
  height: 140%;
}

@media(max-width: 1120px){
  .mediaflex{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 2rem;
  }
  .none_media{
    display: none;
  }
  .mediaflex p{
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 40px;
  }
}
</style>