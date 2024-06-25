<template>
  <div class="container">
    <div>
      <div data-aos="fade-up">
        <div v-for="index in item" :key="index.name"
        >
          <div class="flex flex-col gap-4" data-aos="fade-up" data-aos-anchor-placement="bottom-bottom"
          >
            <h2 class="text-white font-bold text-[25px]">{{index.name}}</h2>
            <div class="text-gray-300 font-medium text-[15px] mb-10 flex flex-col gap-6"
                 data-aos="fade-up" data-aos-anchor-placement="bottom-bottom"
            >
              <p>{{index.desc}}</p>
              <p>{{index.desc2}}</p>
              <p>{{index.desc3}}</p>
              <p>{{index.desc4}}</p>
            </div>
          </div>
        </div>

        <div v-for="word in text" :key="word.name"
        >
          <div data-aos="fade-up">
            <div>
              <h2 class="text-white font-bold text-[25px] mb-4">{{word.name}}</h2>
              <div class="flex flex-col gap-6"
                   data-aos="fade-up" data-aos-anchor-placement="bottom-bottom">
                <div class="flex gap-8 items-center">
                  <span data-v-ed0b00c6="" class="w-[8px] h-[8px] bg-[#00A795] rounded-[50%] flex shrink-0 mt-2 md:-mt-5"></span>
                  <p class="text-gray-300 font-medium text-[15px]">{{word.title1}}</p>
                </div>
                <div class="border-b border-[#39393B] ml-10"></div>

                <div class="flex gap-8 items-center">
                  <span data-v-ed0b00c6="" class="w-[8px] h-[8px] bg-[#00A795] rounded-[50%] flex shrink-0 mt-2 md:-mt-5"></span>
                  <p class="text-gray-300 font-medium text-[15px]">{{word.title2}}</p>
                </div>
                <div class="border-b border-[#39393B] ml-10"></div>

                <div class="flex gap-8 items-center">
                  <span data-v-ed0b00c6="" class="w-[8px] h-[8px] bg-[#00A795] rounded-[50%] flex shrink-0 mt-2 md:-mt-5"></span>
                  <p class="text-gray-300 font-medium text-[15px]">{{word.title3}}</p>
                </div>
                <div class="border-b border-[#39393B] ml-10"></div>

                <div class="flex gap-8 items-center">
                  <span data-v-ed0b00c6="" class="w-[8px] h-[8px] bg-[#00A795] rounded-[50%] flex shrink-0 mt-2 md:-mt-5"></span>
                  <p class="text-gray-300 font-medium text-[15px]">{{word.title4}}</p>
                </div>
                <div class="border-b border-[#39393B] ml-10"></div>

                <div class="flex gap-8 items-center">
                  <span data-v-ed0b00c6="" class="w-[8px] h-[8px] bg-[#00A795] rounded-[50%] flex shrink-0 mt-2 md:-mt-5"></span>
                  <p class="text-gray-300 font-medium text-[15px]">{{word.title5}}</p>
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

const item = [
  {
    id: 1,
    name: "Health",
    desc: "Interim medical examinations throughout the year and consultation with a full-time medical officer are available to employees all year round. The health of all employees is always under control.",
  },
  {
    id: 2,
    name: "UIC values",
    desc: "UIC Group offers its solutions in all aspects of the IT world of any complexity in Uzbekistan. \"UIC Group\" is the address of projects that have their own values ​​and where quality control comes first. The company's activity is aimed at meeting the demand of our customers at the highest level. Our company is ready to serve customers not just as customers, but as partners",
    desc2: "The company differs from classical companies in its focus and system. What matters is not the income, but the result and experience. We are engaged in robotics, digital marketing, game development, maintenance of various software systems.",
    desc3: "The United IT Company team puts quality ahead of financial gain. More precisely, we work with people, not with computers. Feedback from our clients also confirms that UIC takes a responsible approach to the assigned tasks and responsibilities, and maintains a well-coordinated team process.",
    desc4: "After all, we strive to become a leading team in the field of IT, conducting activities based on international standards. Feedback from our clients also confirms that UIC takes a responsible approach to the assigned tasks and responsibilities, and maintains a well-coordinated team process."
  },
  {
    id: 3,
    name: "Corporate Code of the company",
    desc: "Ensuring high standards of corporate governance in practice is very difficult. Therefore, the adoption of a code that summarizes the rules of corporate etiquette is a way to ensure information openness and publicity of the company's activities, with the help of which the company can use it as a means of increasing its corporate attractiveness in the market of its activities.",
    desc2: "The corporate code is valid for each employee of the company, from the degree of obligation to the function of a specific company constitution.",
    desc3: "The corporate code is valid for each employee of the company, from the degree of obligation to the function of a specific company constitution. This code regulates the activities of the company not only by etiquette, but also by general laws. In particular, employees of the company must not take actions that are contrary to or not in the interests of the company, regardless of their position. That is, an employee with a higher competence should not have a negative impact on the opinion of employees whose position is lower than him, force him to perform work that is beyond his competence or contrary to his competence. Administration employees, as well as all employees of the company, use the company's property in the interests of third parties or for personal interests, disclose limited (confidential) information, etc. they do not have the right to pursue (directly or indirectly) any material and / or moral interest.",
  },
]

const text = [
  {
    id: 4,
    name: "About management at UIC",
    title1: "\n" +
        "The main project management tool is Atlassian's products based on the Platinum partnership with UIC Group, Jira is a commercial error tracking system designed to organize interaction with users, although in some cases it is also used for project management. Agile methodology is also used in project management.",
    title2: "\n" +
        "When implementing each new project, automated code analysis is carried out, which helps to find vulnerabilities in the code and timely suppress errors.",
    title3: "\n" +
        "When implementing projects, we use our own project life cycle, which was developed by our team and has huge advantages in terms of time and quality of product creation.",
    title4: "The presence of qualified specialists in the QA testing team, the team is interested in making any product user-friendly, both in terms of functionality and design. To do this, they constantly interact with all members of the development team and constantly compare the result with the given requirements.",
    title5: "\n" +
        "Well-established work with checklists, all these recommendations are difficult to take into account and implement at the checklist design stage. We pay much attention to this mechanism, the better it works and the more benefits it brings to our business. We have been automating work with checklists for many years and have accumulated our own large database of templates that can become the basis for your own checklist",
  }
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