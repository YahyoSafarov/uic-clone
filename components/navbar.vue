<template>
  <div class="wrapper">
    <header class="header" :class="{ active: isHeaderActive }" ref="header">
      <div class="flex items-center justify-center containerr">
        <NuxtLink to="/" class="logo">
          <img src="" class="w-[100px]" alt="" />
          <span class="span">UIC</span>
          <p class="text-[#c5bebe]">Group</p>
        </NuxtLink>

        <nav class="navbar" :class="{ active: isNavbarActive }" ref="navbar">
          <button
            class="nav-close-btn"
            aria-label="close menu"
            @click="toggleNavbar"
          >
            <ion-icon name="close-sharp" aria-hidden="true"
              ><img src="../assets/images/close-large-line.png" alt="no icon"
            /></ion-icon>
          </button>

          <ul class="navbar-list">
            <li>
              <NuxtLink to="/about" class="navbar-link" @click="closeNavbar"
                >About Us</NuxtLink
              >
            </li>
            <li>
              <NuxtLink to="/services" class="navbar-link" @click="closeNavbar"
                >Services</NuxtLink
              >
            </li>
            <li>
              <NuxtLink to="/portfolio" class="navbar-link" @click="closeNavbar"
                >Portfolio</NuxtLink
              >
            </li>
            <li>
              <NuxtLink to="/career" class="navbar-link" @click="closeNavbar"
                >Career</NuxtLink
              >
            </li>
            <li>
              <NuxtLink to="/blog" class="navbar-link" @click="closeNavbar"
                >Blog</NuxtLink
              >
            </li>
            <!--            <li><NuxtLink to="/language" class="navbar-link" @click="closeNavbar">Language</NuxtLink></li>-->
            <li>
              <a
                href="#"
                class="navbar_contact flex gap-4 items-center font-bold text-[25px]"
                @click="closeNavbar"
              >
                <div class="group flex items-center gap-4">
                  <h4
                    class="text-[#c5bebe] duration-150 group-hover:text-white"
                  >
                    +998 71
                  </h4>
                  <h4 class="text-white">200 70 07</h4>
                </div>
              </a>
            </li>
          </ul>
        </nav>

        <!--        <a href="#" class="btn btn-secondary">Join Now</a>-->

        <button
          class="nav-open-btn"
          aria-label="open menu"
          @click="toggleNavbar"
        >
          <span class="line"></span>
          <span class="line"></span>
          <span class="line"></span>
        </button>
      </div>
    </header>
  </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";

/**
 * State variables
 */
const isNavbarActive = ref(false);
const isHeaderActive = ref(false);

/**
 * References to DOM elements
 */
const header = ref(null);
const navbar = ref(null);

/**
 * Toggle navbar function
 */
const toggleNavbar = () => {
  isNavbarActive.value = !isNavbarActive.value;
};

/**
 * Close navbar function
 */
const closeNavbar = () => {
  isNavbarActive.value = false;
};

/**
 * Scroll handler to update header state
 */
const handleScroll = () => {
  isHeaderActive.value = window.scrollY >= 100;
};

/**
 * Add event listeners on component mount
 */
onMounted(() => {
  window.addEventListener("scroll", handleScroll);
});

/**
 * Clean up event listeners on component unmount
 */
onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script>

<style lang="scss" scoped>
/*-----------------------------------*\
  #HEADER
\*-----------------------------------*/

.header .btn {
  display: none;
}

.header {
  background-color: var(--white);
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  padding-block: 10px;
  box-shadow: var(--shadow-1);
  z-index: 9999;
}

.logo {
  color: var(--rich-black-fogra-29-1);
  font-family: var(--ff-catamaran);
  font-size: 3.5rem;
  font-weight: var(--fw-900);
  display: flex;
  align-items: center;
  margin-inline-start: -65px;
}

.logo ion-icon {
  color: var(--coquelicot);
  font-size: 40px;
  //transform: rotate(90deg) translate(-2px, -5px);
}

.nav-open-btn {
  background-color: #00a795;
  padding: 15px 10px;
  border-radius: var(--radius-8);
}

.nav-open-btn .line {
  background-color: var(--white);
  width: 20px;
  height: 1.7px;
}

.nav-open-btn .line:not(:last-child) {
  margin-block-end: 6px;
}

.nav-open-btn .line:nth-child(2) {
  width: 25px;
  margin-inline-start: auto;
}

.navbar {
  background-color: #1a8377;
  color: white;
  position: fixed;
  top: 100%;
  left: 0;
  width: 100%;
  height: 100%;
  display: grid;

  place-content: center;
  visibility: hidden;
  transition: 0.25s var(--cubic-in);
}

.navbar.active {
  visibility: visible;
  transform: translateY(-100%);
  transition: 0.5s var(--cubic-out);
}

.nav-close-btn {
  position: absolute;
  top: 10px;
  right: 15px;
  background-color: var(--rich-black-fogra-29-1);
  color: var(--white);
  font-size: 40px;
  padding: 10px;
  border-radius: var(--radius-8);
}

.navbar-link {
  font-family: var(--ff-catamaran);
  font-size: 20px;
  text-align: center;
  padding-block: 10px;
  margin-block-end: 20px;
  transition: var(--transition-1);
  color: white;
}

.navbar-link:is(:hover, :focus, .active) {
  color: var(--rich-black-fogra-29-1);
}

.navbar_contact span:hover {
  color: white;
}

/*-----------------------------------*\
  #MEDIA QUERIES
\*-----------------------------------*/

/**
 * responsive for larger than 575px screen
 */

@media (min-width: 575px) {
  /**
   * CUSTOM PROPERTY
   */

  :root {
    /**
     * typography
     */

    --fs-1: 5.8rem;
    --fs-2: 4rem;
  }

  /**
   * REUSED STYLE
   */

  .containerr {
    max-width: 1440px;
    width: 100%;
    margin-inline: auto;
  }

  .hero-subtitle,
  .section-subtitle {
    font-size: var(--fs-5);
  }

  /**
   * HEADER
   */

  .header .containerr {
    display: flex;
    max-width: unset;
    padding-inline: 30px;
  }

  /**
   * HERO
   */

  .hero-content {
    padding-inline: 40px;
  }

  .hero-subtitle .strong {
    padding-block: 6px;
  }

  .hero::after {
    height: 340px;
  }

  .abs-img-1 {
    top: 130px;
    right: -10px;
    width: 230px;
  }

  .abs-img-2 {
    bottom: 20px;
    left: -40px;
    width: 310px;
  }

  /**
   * ABOUT
   */

  .about .wrapper {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    gap: 40px;
  }

  .about-coach {
    margin-block-end: 0;
  }

  /**
   * VIDEO
   */

  .video-card .card-title {
    --fs-3: 3.5rem;
  }

  /**
   * FOOTER
   */

  .footer-top .containerr {
    grid-template-columns: 1fr 1fr;
    column-gap: 25px;
  }
}

/**
 * responsive for larger than 768px screen
 */

@media (min-width: 768px) {
  /**
   * CUSTOM PROPERTY
   */

  :root {
    /**
     * typography
     */

    --fs-2: 4.5rem;
  }

  /**
   * REUSED STYLE
   */

  .containerr {
    max-width: 720px;
  }

  .scrollbar-item {
    min-width: calc(50% - 12.5px);
  }

  /**
   * HERO
   */

  .hero-banner {
    max-width: max-content;
    margin-inline: auto;
  }

  .abs-img-1 {
    top: 140px;
    right: 50px;
  }

  /**
   * FOOTER
   */

  .footer-bottom .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .footer-bottom-list {
    margin-block-start: 0;
  }
}

/**
 * responsive for larger than 992px screen
 */

@media (min-width: 1120px) {
  /**
   * REUSED STYLE
   */

  .container,
  .header .containerr {
    max-width: 960px;
  }

  /**
   * HEADER
   */

  .nav-open-btn,
  .nav-close-btn {
    display: none;
  }

  .header .btn {
    display: block;
  }

  .header {
    background-color: transparent;
    box-shadow: none;
    padding-block: 30px;
    transition: var(--transition-1);
  }

  .header.active {
    transform: translateY(-100%);
    background-color: rgba(0, 0, 0, 0.4);
    -webkit-backdrop-filter: blur(20px);
    backdrop-filter: blur(20px);
    padding-block: 20px;
    box-shadow: var(--shadow-1);
    animation: slideIn 0.5s ease forwards;
  }

  @keyframes slideIn {
    0% {
      transform: translateY(-100%);
    }
    100% {
      transform: translateY(0);
    }
  }

  .header .containerr {
    gap: 40px;
  }

  .header .logo {
    color: var(--white);
  }

  .header.active .logo {
    color: #1a8377;
  }

  .navbar,
  .navbar.active {
    all: unset;
    margin-inline: auto;
  }

  .navbar-list {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 45px;
  }

  .navbar-link {
    color: #c5bebe;
    font-size: 20px;
    padding: 0 10px;
    margin-block-end: 0;
  }

  .header.active .navbar-link {
    color: #c5bebe;
  }

  .header .navbar-link:is(:hover, :focus, .active) {
    color: white;
  }

  .header.active .btn {
    background-color: #00a795;
    color: var(--white);
  }

  .header.active .btn:is(:hover, :focus) {
    background-color: var(--rich-black-fogra-29-1);
  }

  /**
   * HERO
   */

  .hero-content {
    padding-inline: 0;
    margin-block-end: 0;
  }

  .hero-subtitle,
  .hero .btn {
    margin-inline: 0;
  }

  .hero::after {
    width: 330px;
    height: 100%;
    left: auto;
    right: 0;
  }

  /**
   * ABOUT
   */

  .about .container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    gap: 50px;
  }

  .about-banner {
    margin-block-end: 0;
  }

  .about .wrapper {
    gap: 30px;
  }

  /**
   * FOOTER
   */

  .footer-top .container {
    grid-template-columns: 0.85fr 0.5fr 1fr 0.85fr;
    column-gap: 50px;
  }
}

/**
 * responsive for larger than 1200px screen
 */

@media (min-width: 1200px) {
  /**
   * CUSTOM PROPERTY
   */

  :root {
    /**
     * typography
     */

    --fs-1: 7rem;
    --fs-2: 5.5rem;
    --fs-4: 2.2rem;
    --fs-5: 2rem;

    /**
     * spacing
     */

    --section-padding: 120px;
  }

  /**
   * REUSED STYLE
   */

  .containerr,
  .header .containerr {
    max-width: 1440px;
  }

  .btn {
    padding: 18px 45px;
    border-radius: var(--radius-10);
  }

  .section-subtitle {
    --fs-5: 2.2rem;
  }

  .has-scrollbar {
    gap: 30px;
  }

  .scrollbar-item {
    min-width: calc(33.33% - 20px);
  }

  /**
   * HEADER
   */

  .header .containerr {
    padding-inline: 0;
  }

  /**
   * HERO
   */

  .hero::after {
    width: 420px;
  }

  .hero .section-text {
    --fs-6: 1.8rem;
  }

  .abs-img-1 {
    top: 170px;
    right: -30px;
    width: 260px;
  }

  .abs-img-2 {
    bottom: 60px;
    left: -80px;
    width: 360px;
  }

  /**
   * ABOUT
   */

  .about .wrapper {
    gap: 40px;
  }

  /**
   * CLASS, BLOG
   */

  :is(.class-card, .blog-card) .card-content {
    padding: 30px;
  }

  .blog-card .card-meta {
    padding: 15px 30px;
  }

  /**
   * FOOTER
   */

  .footer-top .containerr {
    grid-template-columns: 1fr 0.6fr 0.9fr 1fr;
  }
}
</style>
