<template>
  <div class="flex justify-between">
    <div class="font-semibold dark:text-cyan-500 duration-1000">
      <a href="https://github.com/inspect07" target="_blank">&#64;Inspect07</a>
    </div>
    <div class="flex space-x-2 items-center">
      <div :class="`mode ${isDark ? 'dark-mode' : ''}`" @click="mode">
        <div class="switch">
          <div :class="`switch-inner ${isDark ? 'dark-mode' : ''}`"></div>
        </div>
      </div>
      <div
        :class="`darkmode-animate bg-slate-900  ${isDark ? 'active' : ''}`"
      ></div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { useDark, useToggle } from "@vueuse/core";

const isDark = useDark();
const toggleDark = useToggle(isDark);

const mode = () => {
  toggleDark();
};
</script>

<style lang="scss" scoped>
.mode {
  width: 45px;
  height: 25px;
  padding: 5px;
  background: rgb(17 24 39);
  border-radius: 50px;
  cursor: pointer;
  overflow: hidden;

  .switch-inner {
    position: relative;
    width: 15px;
    height: 15px;
    background: #ffc207;
    border-radius: 50px;
    transition: all 0.6s;

    &::before {
      content: " ";
      position: absolute;
      top: 0;
      left: -60%;
      width: 100%;
      height: 100%;
      background: var(--dark-mode);
      z-index: 999;
      border-radius: 50px;
      transform: scale(0);
      transition: all 0.6s;
    }

    &.dark-mode {
      transform: translateX(calc(45px - 25px));
      background: #ffc207;

      &::before {
        left: -55%;
        transform: scale(1);
        background: #fff;
      }
    }
  }

  &.dark-mode {
    background: #fff;
  }
}

.resume {
  padding-top: 3px;
  padding-bottom: 3px;
  text-transform: capitalize;
}

.darkmode-animate {
  z-index: -999;
  position: absolute;
  width: 99%;
  height: 500vh;
  left: 0;
  clip-path: circle(0% at 120% 25%);
  transition: clip-path 1.8s ease;

  &.active {
    clip-path: circle(200% at 98% 9%);
  }
}
</style>
