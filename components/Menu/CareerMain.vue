<template>
  <div class="">
    <div class="container pb-44 mt-28">
      <div class="hero">
        <section>
          <div class="content place-items-center">
            <h2>CAREER</h2>
          </div>
          <div>
            <p class="font-bold text-white text-[80px] -mt-20">CAREER</p>
          </div>
        </section>
      </div>
    </div>
  </div>

</template>

<script setup>

</script>

<style lang="scss" scoped>
.hero {
  text-align: center;
  padding-block-start: calc(var(--section-padding) + 150px);
  padding-block-end: 0;
  overflow: hidden;
}

@import url("https://fonts.googleapis.com/css?family=Poppins:100,200,300,400,500,600,700,800,900");



.content {
  display: flex;
  align-items: center;
  justify-content: center;
}


.content h2 {
  color: #fff;
  font-size: 12em;
  font-weight: 800;
  position: absolute;
}

.content h2:nth-child(1) {
  color: transparent;
  -webkit-text-stroke: 2px #ffffff1a;
}

.content h2:nth-child(2) {
  color: #c19bf5;
  animation: animate 4s ease-in-out infinite;
}

@keyframes animate {
  0%,
  100% {
    clip-path: polygon(
            0% 45%,
            16% 44%,
            33% 50%,
            54% 60%,
            70% 61%,
            84% 59%,
            100% 52%,
            100% 100%,
            0% 100%
    );
  }

  50% {
    clip-path: polygon(
            0% 60%,
            15% 65%,
            34% 66%,
            51% 62%,
            67% 50%,
            84% 45%,
            100% 46%,
            100% 100%,
            0% 100%
    );
  }
}

</style>