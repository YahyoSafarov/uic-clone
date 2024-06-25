<template>
  <div class="container py-20">
    <div class="flex gap-[6rem]">
      <div v-for="item in navigation" :key="item.name" :href="item.href"
      >
        <div class="mb-10">
          <div><NuxtLink to="/about" class="font-bold text-[20px]">{{item.name}}</NuxtLink></div>
        </div>
    </div>
    </div>

    <div class="flex  gap-20 items-center">
      <ul class="flex items-center gap-[1rem]">
        <li><a href="#"><img src="https://uic.group/uic-images/socials/facebook.svg" alt=""></a></li>
        <li><a href="#"><img src="https://uic.group/uic-images/socials/twitter.svg" alt=""></a></li>
        <li><a href="#"><img src="https://uic.group/uic-images/socials/instagram.svg" alt=""></a></li>
        <li><a href="#"><img src="https://uic.group/uic-images/socials/telegram.svg" alt=""></a></li>
        <li><a href="#"><img src="https://uic.group/uic-images/socials/linkedin.svg" alt=""></a></li>
        <li><a href="#"><img src="https://uic.group/uic-images/socials/behance.svg" alt=""></a></li>
        <li><a href="#"><img src="https://uic.group/uic-images/socials/dribbble.svg" alt=""></a></li>
        <li><a href="#"><img src="https://uic.group/uic-images/socials/trustpilot.svg" alt=""></a></li>
        <li><a href="#"><img src="https://uic.group/uic-images/socials/yelp.svg" alt=""></a></li>
      </ul>

      <div class="flex gap-6 items-center cursor-pointer">
        <div class="flex gap-4 items-center">
          <i data-v-56c03d90="" data-v-34700754="" class="icon hover:text-red-500 text-white"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect width="24" height="24" rx="12" fill="white" fill-opacity="0.3"></rect>
            <path fill-rule="evenodd" clip-rule="evenodd" d="M12 4.8C8.02355 4.8 4.8 8.02355 4.8 12C4.8 15.9765 8.02355 19.2 12 19.2C13.1511 19.2 14.2367 18.9305 15.1995 18.4521C15.6446 18.2309 16.1847 18.4124 16.4059 18.8575C16.6272 19.3026 16.4456 19.8428 16.0005 20.064C14.7944 20.6634 13.4352 21 12 21C7.02943 21 3 16.9705 3 12C3 7.02943 7.02943 3 12 3C16.9705 3 21 7.02943 21 12V12.9C21 14.1681 20.6826 15.1818 20.0883 15.8949C19.485 16.6188 18.663 16.95 17.85 16.95C16.7458 16.95 15.6292 16.328 15.0691 15.291C14.2651 16.0411 13.1862 16.5 12 16.5C9.51472 16.5 7.5 14.4853 7.5 12C7.5 9.51472 9.51472 7.5 12 7.5C13.013 7.5 13.9479 7.83475 14.7 8.39967C14.7002 7.90277 15.103 7.5 15.6 7.5C16.0971 7.5 16.5 7.90295 16.5 8.4V13.8C16.5 14.5955 17.1626 15.15 17.85 15.15C18.162 15.15 18.465 15.0312 18.7055 14.7426C18.9549 14.4432 19.2 13.8819 19.2 12.9V12C19.2 8.02355 15.9765 4.8 12 4.8ZM14.7 12C14.7 10.5088 13.4912 9.3 12 9.3C10.5088 9.3 9.3 10.5088 9.3 12C9.3 13.4912 10.5088 14.7 12 14.7C13.4912 14.7 14.7 13.4912 14.7 12Z" fill="white"></path>
          </svg>
          </i>
          <p class="duration-300 font-bold hover:text-white">info@uic.group</p>
        </div>

        <div class="flex items-center gap-4 cursor-pointer">
          <i data-v-56c03d90="" data-v-34700754="" class="icon hover:text-red-500 text-white"><svg width="25" height="24" viewBox="0 0 25 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect x="0.427979" width="24" height="24" rx="12" fill="white" fill-opacity="0.3"></rect>
            <path d="M13.3975 13.6577C13.1606 13.8944 12.9237 14.2495 12.7461 14.5455C11.6802 13.7168 10.7327 12.7106 9.90364 11.7044C10.2589 11.5269 10.555 11.2901 10.7919 11.0534C11.9762 9.86958 11.5617 8.33068 10.3774 7.14691C9.19303 5.96314 7.7126 5.48963 6.46904 6.73259C5.22548 7.97555 5.10705 10.1063 6.05452 11.4677C7.77182 14.072 10.3774 16.6763 12.9829 18.3927C14.4041 19.3398 16.536 19.1622 17.7203 17.9784C18.9047 16.7946 18.4901 15.2557 17.3058 14.072C16.1214 12.8882 14.5818 12.4147 13.3975 13.6577Z" stroke="white" stroke-width="1.6" stroke-miterlimit="10" stroke-linejoin="round"></path>
            <path d="M19.428 11C19.428 7.66667 16.7613 5 13.428 5" stroke="white" stroke-width="1.6" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
            <path d="M16.428 11C16.428 9.34043 15.081 8 13.428 8" stroke="white" stroke-width="1.6" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"></path>
          </svg>
          </i>
          <p class=" duration-300 font-bold hover:text-white">+998 71 200 70 07</p>
        </div>
      </div>


    </div>

    <div class="border-b-[2px] border-[#666] mt-14"></div>
  </div>
</template>

<script setup>
const navigation = [
  {
    id: 1,
    name: "About us",
    icon: "https://uic.group/uic-images/socials/facebook.svg",
    src: "",
    text: "info@uic.group",
    href: "/about"
  },
  {
    id: 2,
    name: "Sevices",
    icon: "https://uic.group/uic-images/socials/facebook.svg",
    src: "",
    text: "info@uic.group",
    href: "/about"
  },
  {
    id: 3,
    name: "Portfolio",
    icon: "https://uic.group/uic-images/socials/facebook.svg",
    src: "",
    text: "info@uic.group",
    href: "/about"
  },
  {
    id: 4,
    name: "Career",
    icon: "https://uic.group/uic-images/socials/facebook.svg",
    src: "",
    text: "info@uic.group",
    href: "/about"
  },
  {
    id: 5,
    name: "Blog",
    icon: "https://uic.group/uic-images/socials/facebook.svg",
    src: "",
    text: "info@uic.group",
    href: "/about"
  },
]
</script>

<style lang="scss" scoped>
.container{
  max-width: 1360px;
}



ul li {
  list-style: none;
}

ul li  a {
  position: relative;
  display: flex;
  width: 44px;
  height: 44px;
  align-items: center;
  justify-content: center;;
  background: #333;
  border-radius: 50%;
  font-size: 30px;
  color: #666;
  transition: .5s;
}

ul li a:before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border-radius: 50%;
  background: #1a8377;
  transition: .5s;
  transform: scale(.9);
  z-index: -1;
}

ul li a:hover:before {
  transform: scale(1.1);
  box-shadow: 0 0 15px #1a8377;
}

ul li a:hover {
  color: #ffee10;
  box-shadow: 0 0 5px #1a8377;
  text-shadow: 0 0 5px #1a8377;
  background: #00a795;
}
</style>