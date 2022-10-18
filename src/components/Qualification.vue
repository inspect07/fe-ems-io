<template>
  <div class="max-w-7xl m-center pt-20 pb-20">
    <div class="qualification text-center mt-10">
      <h2 class="text-5xl dark:text-white">Qualification</h2>
      <span class="f-gray text-sm dark:text-white">My Personal Journey</span>
    </div>
    <div class="qualification-details qualification-tab flex flex-col mt-20">
      <div class="flex justify-center">
        <div class="work-tab tabs w-1/4 text-center">
          <h2
            class="text-lg cursor-pointer underline underline-offset-1 font-extrabold dark:text-white"
            :class="`${active == 'work' ? 'active' : ''}`"
            @click="switchTo('work')"
          >
            Work
          </h2>
        </div>
        <div class="education-tab tabs w-1/4 text-center">
          <h2
            class="text-lg cursor-pointer underline underline-offset-1 font-extrabold dark:text-white"
            :class="`${active == 'education' ? 'active' : ''}`"
            @click="switchTo('education')"
          >
            Education
          </h2>
        </div>
      </div>
      <div class="tabs-content">
        <Work v-if="active == 'work'" />
        <Education v-else />
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref } from "@vue/runtime-dom";
import Work from "@/components/Work.vue";
import Education from "@/components/Education.vue";

const active = ref("work");

const switchTo = (tab: any) => {
  active.value = tab;
};
</script>
