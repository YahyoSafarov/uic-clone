<template>
  <div class="container mt-24">
    <div>
      <div class="flex flex-col gap-10">
        <div v-for="index in text" :key="index.name"
        >
          <div class="text-start">
            <h1 class="text-white font-medium text-[25px] mb-7">{{index.name}}</h1>
            <div class="text-[#999] text-[14px]">
              <p>{{index.title1}}</p>
              <p>{{index.title2}}</p>
              <p>{{index.title3}}</p>
              <p>{{index.title4}}</p>
              <p>{{index.title5}}</p>
              <p>{{index.title6}}</p>
              <p>{{index.title7}}</p>
              <p>{{index.title8}}</p>
              <p>{{index.title9}}</p>
              <p>{{index.title10}}</p>
              <p>{{index.title11}}</p>
              <p>{{index.title12}}</p>
              <p>{{index.title13}}</p>
            </div>

          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const text = [
  {
    id: 1,
    name: "Requirements",
    title1: 'Support and improvement of existing projects, as well as the introduction of new functionality;',
    title2: 'Teamwork with other developers, QA testers, backend programmers and UI/UX designers.',
  },
  {
    id: 2,
    name: 'Tasks',
    title1: 'Knowledge of the application structure of PWA(Progressive Web App), SPA(Single Page Application), SSR(Server-Side Rendering), MF(Mutual Funds);',
    title2: 'Understanding the principles of SOLID, KISS, DRY.',
    title3: 'More than 2 years of work experience.(active development for more than 1 year);',
    title4: 'Knowledge of JavaScript and its basic concepts (prototypical inheritance, event loop, closures, this keyword, etc.);',
    title5: 'Knowledge of modern methods of writing code in JavaScript and TypeScript;',
    title6: 'Work experience with Vue.js 2.3, Pinia, Vue Router;',
    title7: 'Ability to work with Axios and API;',
    title8: 'Knowledge of Tailwind CSS and good layout skills;',
    title9: 'Experience working with NPM/ Yarn for package management;',
    title10: 'Experience working with project builders in Vue, Vue CLI, Webpack, Rollup;',
    title11: 'Knowledge of Git, Shell Commands, Git Flow;',
    title12: 'Experience working with Nuxt.js;',
    title13: 'Willingness to constantly learn and explore new technologies.',
  },
  {
    id: 3,
    name: 'Conditions',
    title1: 'Knowledge of the application structure of PWA(Progressive Web App), SPA(Single Page Application), SSR(Server-Side Rendering), MF(Mutual Funds);',
    title2: 'Understanding the principles of SOLID, KISS, DRY.',
    title3: 'More than 2 years of work experience.(active development for more than 1 year);',
    title4: 'Friendly and supportive atmosphere in the team, regular team events, team building, including marathons and quizzes;',
    title5: 'The company is proud to provide its employees with the most modern and high-quality equipment for work;',
    title6: 'A modern office with work facilities;',
    title7: 'Timely payment of labor, including a system of bonuses for outstanding results;',
    title8: 'Employment in accordance with the Labor Code of the Republic of Uzbekistan.\n' +
        'If you are ready to join our team and contribute to the development of innovative projects, please send your resume\n' +
        '\n' +
        'For more information about our capabilities, please follow this link. (https://uic.group/about)',
  },
]
</script>

<style lang="scss" scoped>
.container{
  max-width: 1170px;
}
</style>