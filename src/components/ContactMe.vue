<template>
  <div class="max-w-7xl m-center pt-1 pb-20">
    <div class="about-me text-center mt-10 md:mt-32">
      <h2
        class="text-5xl dark:text-white"
        data-aos="fade-right"
        data-aos-duration="500"
      >
        Get in Touch
      </h2>
      <h4
        class="f-gray text-lg dark:text-white pt-9 w-9/12 m-auto"
        data-aos="fade-right"
        data-aos-duration="500"
      >
        Although I’m not currently looking for any new opportunities, my inbox
        is always open. Whether you have a question or just want to say hi, I’ll
        try my best to get back to you!
      </h4>
    </div>
    <div
      class="flex justify-center items-center mt-24"
      data-aos="fade-right"
      data-aos-duration="500"
    >
      <button class="button dark:text-white dark:border-white w-36">
        <a href="mailto:eman15santiago@gmail.com">Say Hi</a>
      </button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
/* From uiverse.io */
.button {
  display: inline-block;
  padding: 12px 24px;
  border: 1px solid;
  border-radius: 4px;
  transition: all 0.2s ease-in;
  position: relative;
  overflow: hidden;
  font-size: 19px;
  z-index: 1;
}

.button:before {
  content: "";
  position: absolute;
  left: 50%;
  transform: translateX(-50%) scaleY(1) scaleX(1.25);
  top: 100%;
  width: 140%;
  height: 180%;
  background-color: rgba(0, 0, 0, 0.05);
  border-radius: 50%;
  display: block;
  transition: all 0.5s 0.1s cubic-bezier(0.55, 0, 0.1, 1);
  z-index: -1;
}

.button:after {
  content: "";
  position: absolute;
  left: 55%;
  transform: translateX(-50%) scaleY(1) scaleX(1.45);
  top: 180%;
  width: 160%;
  height: 190%;
  background-color: #39bda7;
  border-radius: 50%;
  display: block;
  transition: all 0.5s 0.1s cubic-bezier(0.55, 0, 0.1, 1);
  z-index: -1;
}

.button:hover {
  color: #ffffff;
  border: 1px solid #39bda7;
}

.button:hover:before {
  top: -35%;
  background-color: #39bda7;
  transform: translateX(-50%) scaleY(1.3) scaleX(0.8);
}

.button:hover:after {
  top: -45%;
  background-color: #39bda7;
  transform: translateX(-50%) scaleY(1.3) scaleX(0.8);
}
</style>
