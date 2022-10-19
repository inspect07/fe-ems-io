<script setup lang="ts">
import Header from "@/components/Header.vue";
import Hero from "@/components/Hero.vue";
import AboutMe from "@/components/AboutMe.vue";
import Skills from "@/components/Skills.vue";
import Qualification from "@/components/Qualification.vue";
import Portfolio from "@/components/Portfolio.vue";
import Footer from "@/components/Footer.vue";
import ContactMe from "@/components/ContactMe.vue";

import { ref, onMounted } from "@vue/runtime-dom";
import AOS from "aos";

const loading = ref(true);

onMounted(() => {
  AOS.init({});
  setTimeout(() => {
    loading.value = false;
  }, 5000);
});
</script>

<template>
  <main class="dark:bg-gray-900 main">
    <div class="loader-wrapper" v-if="loading">
      <div class="loader">
        <svg viewBox="0 0 80 80">
          <circle id="test" cx="40" cy="40" r="32"></circle>
        </svg>
      </div>

      <div class="loader triangle">
        <svg viewBox="0 0 86 80">
          <polygon points="43 8 79 72 7 72"></polygon>
        </svg>
      </div>

      <div class="loader">
        <svg viewBox="0 0 80 80">
          <rect x="8" y="8" width="64" height="64"></rect>
        </svg>
      </div>
    </div>
    <div
      class="md:px-20 p-5 lg:px-5"
      style="max-width: 1280px; margin: auto"
      v-else
    >
      <Header />
      <Hero />
      <Portfolio />
      <AboutMe />
      <Skills />
      <Qualification />
      <ContactMe />
    </div>
    <Footer v-if="!loading" />
  </main>
</template>

<style lang="scss" scoped>
.loader-wrapper {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;

  .loader {
    --path: #2f3545;
    --dot: #5628ee;
    --duration: 3s;
    width: 44px;
    height: 44px;
    position: relative;

    &::before {
      content: "";
      width: 6px;
      height: 6px;
      border-radius: 50%;
      position: absolute;
      display: block;
      background: var(--dot);
      top: 37px;
      left: 19px;
      transform: translate(-18px, -18px);
      animation: dotRect var(--duration) cubic-bezier(0.785, 0.135, 0.15, 0.86)
        infinite;
    }
  }
}

.loader svg {
  display: block;
  width: 100%;
  height: 100%;
}

.loader svg rect,
.loader svg polygon,
.loader svg circle {
  fill: none;
  stroke: var(--path);
  stroke-width: 10px;
  stroke-linejoin: round;
  stroke-linecap: round;
}

.loader svg polygon {
  stroke-dasharray: 145 76 145 76;
  stroke-dashoffset: 0;
  animation: pathTriangle var(--duration) cubic-bezier(0.785, 0.135, 0.15, 0.86)
    infinite;
}

.loader svg rect {
  stroke-dasharray: 192 64 192 64;
  stroke-dashoffset: 0;
  animation: pathRect 3s cubic-bezier(0.785, 0.135, 0.15, 0.86) infinite;
}

.loader svg circle {
  stroke-dasharray: 150 50 150 50;
  stroke-dashoffset: 75;
  animation: pathCircle var(--duration) cubic-bezier(0.785, 0.135, 0.15, 0.86)
    infinite;
}

.loader.triangle {
  width: 48px;
}

.loader.triangle:before {
  left: 21px;
  transform: translate(-10px, -18px);
  animation: dotTriangle var(--duration) cubic-bezier(0.785, 0.135, 0.15, 0.86)
    infinite;
}

@keyframes pathTriangle {
  33% {
    stroke-dashoffset: 74;
  }

  66% {
    stroke-dashoffset: 147;
  }

  100% {
    stroke-dashoffset: 221;
  }
}

@keyframes dotTriangle {
  33% {
    transform: translate(0, 0);
  }

  66% {
    transform: translate(10px, -18px);
  }

  100% {
    transform: translate(-10px, -18px);
  }
}

@keyframes pathRect {
  25% {
    stroke-dashoffset: 64;
  }

  50% {
    stroke-dashoffset: 128;
  }

  75% {
    stroke-dashoffset: 192;
  }

  100% {
    stroke-dashoffset: 256;
  }
}

@keyframes dotRect {
  25% {
    transform: translate(0, 0);
  }

  50% {
    transform: translate(18px, -18px);
  }

  75% {
    transform: translate(0, -36px);
  }

  100% {
    transform: translate(-18px, -18px);
  }
}

@keyframes pathCircle {
  25% {
    stroke-dashoffset: 125;
  }

  50% {
    stroke-dashoffset: 175;
  }

  75% {
    stroke-dashoffset: 225;
  }

  100% {
    stroke-dashoffset: 275;
  }
}

.loader {
  display: inline-block;
  margin: 0 16px;
}
</style>
