<template>
  <div class="max-w-7xl m-center pt-48">
    <div
      class="skills text-center mt-10"
      data-aos="fade-up"
      data-aos-delay="100"
      data-aos-duration="800"
    >
      <h2 class="text-5xl dark:text-white">Skills</h2>
      <span class="f-gray text-sm dark:text-white">My Technical Level</span>
    </div>
    <div class="skill-details flex mt-20 flex-col lg:flex-row lg:gap-10">
      <div
        data-aos="fade-down"
        data-aos-duration="1000"
        data-aos-delay="200"
        class="lg:w-1/3 md:w-96 md:m-auto md:mb-16 card bg-white drop-shadow-2xl dark:bg-slate-800"
      >
        <h2 class="pt-7 pl-5 flex items-center">
          <font-awesome-icon
            class="fa-2xl pr-3 f-blue w-20"
            :icon="['fas', 'code']"
          />
          <div class="flex flex-col">
            <h2 class="text-xl dark:text-white">Frontend Developer</h2>
            <span class="text-sm f-gray dark:text-white"
              >More than 4 years</span
            >
          </div>
        </h2>
        <div
          class="description grid grid-cols-4 gap-4 m-auto lg:px-10 px-5 pt-10"
        >
          <div class="p-1 card-mini">
            <img
              src="https://seeklogo.com/images/V/vuejs-logo-17D586B587-seeklogo.com.png"
              class="h-14"
              alt="VUEJS"
            />
            <span class="dark:text-white">VueJs</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://www.logo.wine/a/logo/React_(web_framework)/React_(web_framework)-Logo.wine.svg"
              class="h-14"
              alt="ReactJs"
            />
            <span class="dark:text-white">ReactJs</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/JavaScript-logo.png/600px-JavaScript-logo.png?20120221235433"
              class="h-14"
              alt="JavaScript"
            />
            <span class="dark:text-white">JavaScript</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Typescript_logo_2020.svg/512px-Typescript_logo_2020.svg.png?20210506173343"
              class="h-14"
              alt="TypeScript"
            />
            <span class="dark:text-white">TypeScript</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ae/Nuxt_logo.svg/512px-Nuxt_logo.svg.png?20201218211241"
              class="h-14"
              alt="NuxtJs"
            />
            <span class="dark:text-white">NuxtJs</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://mui.com/static/logo.png"
              class="h-14"
              alt="MaterialUI"
            />
            <span class="dark:text-white">MaterialUI</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/Tailwind_CSS_Logo.svg/600px-Tailwind_CSS_Logo.svg.png?20211001194333"
              class="h-14"
              alt="Tailwind"
            />
            <span class="dark:text-white">Tailwind</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://seeklogo.com/images/B/bootstrap-logo-3C30FB2A16-seeklogo.com.png"
              class="h-14"
              alt="Bootstrap"
            />
            <span class="dark:text-white">Bootstrap</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/130px-HTML5_logo_and_wordmark.svg.png"
              alt="HTML5"
              class="h-14"
            />
            <span class="dark:text-white">HTML5</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/CSS3_logo_and_wordmark.svg/120px-CSS3_logo_and_wordmark.svg.png"
              class="h-14"
              alt="CSS"
            />
            <span class="dark:text-white">CSS</span>
          </div>
        </div>
      </div>
      <div
        data-aos="fade-down"
        data-aos-duration="1000"
        data-aos-delay="400"
        class="lg:w-1/3 md:w-96 md:m-auto md:mb-16 card bg-white drop-shadow-2xl dark:bg-slate-800"
      >
        <h2 class="pt-7 pl-5 flex items-center">
          <font-awesome-icon
            class="fa-2xl pr-3 f-blue w-20"
            :icon="['fas', 'code-branch']"
          />
          <div class="flex flex-col">
            <h2 class="text-xl dark:text-white">Backend Developer</h2>
            <span class="text-sm f-gray dark:text-white"
              >More than 2 years</span
            >
          </div>
        </h2>
        <div
          class="description grid grid-cols-4 gap-4 m-auto lg:px-10 px-5 pt-10"
        >
          <div class="p-1 card-mini">
            <img
              src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Laravel.svg/121px-Laravel.svg.png"
              class="h-14"
              alt="Laravel"
            />
            <span class="dark:text-white">Laravel</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://cdn-icons-png.flaticon.com/512/5968/5968332.png"
              class="h-14"
              alt="PHP"
            />
            <span class="dark:text-white">PHP</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://www.freepnglogos.com/uploads/logo-mysql-png/logo-mysql-mysql-logo-png-images-are-download-crazypng-21.png"
              class="h-14"
              alt="Mysql"
            />
            <span class="dark:text-white">Mysql</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRK_A4ygFZawvqLFvYUYfssFpgwAfCGZ7Xs_Ka4hDnmgA&s"
              class="h-14"
              alt="AWS"
            />
            <span class="dark:text-white">AWS</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://seeklogo.com/images/D/docker-logo-CF97D0124B-seeklogo.com.png"
              class="h-14"
              alt="Docker"
            />
            <span class="dark:text-white">Docker</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://cms-assets.tutsplus.com/uploads/users/433/posts/23928/preview_image/Untitled.png"
              class="h-14"
              alt="Laravel Lumen"
            />
            <span class="dark:text-white">Laravel Lumen</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://cdn3.iconfinder.com/data/icons/social-media-2169/24/social_media_social_media_logo_codeigniter-512.png"
              class="h-14"
              alt="CodeIgniter"
            />
            <span class="dark:text-white">CodeIgniter</span>
          </div>
        </div>
      </div>
      <div
        data-aos="fade-down"
        data-aos-duration="1000"
        data-aos-delay="600"
        class="lg:w-1/3 md:w-96 md:m-auto md:mb-16 card bg-white drop-shadow-2xl dark:bg-slate-800"
      >
        <h2 class="pt-7 pl-5 flex items-center">
          <font-awesome-icon
            class="fa-2xl pr-3 f-blue w-20"
            :icon="['fas', 'brain']"
          />
          <div class="flex flex-col">
            <h2 class="text-xl dark:text-white">Others</h2>
            <span class="text-sm f-gray dark:text-white">Acquired Skills</span>
          </div>
        </h2>
        <div
          class="description grid grid-cols-4 gap-4 m-auto lg:px-10 px-5 pt-10"
        >
          <div class="p-1 card-mini">
            <img
              src="https://seeklogo.com/images/G/github-logo-5F384D0265-seeklogo.com.png"
              class="h-14"
              alt="Git"
            />
            <span class="dark:text-white">Git</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://cdn.icon-icons.com/icons2/2699/PNG/512/atlassian_jira_logo_icon_170511.png"
              class="h-14"
              alt="Jira"
            />
            <span class="dark:text-white">Jira</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://cdn.sanity.io/images/599r6htc/localized/46a76c802176eb17b04e12108de7e7e0f3736dc6-1024x1024.png?w=670&h=670&q=75&fit=max&auto=format"
              class="h-14"
              alt="Figma"
            />
            <span class="dark:text-white">Figma</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://assets-global.website-files.com/60058af53d79fbd8e14841ea/6016c5d7eaca0a225f621fd0_Tg7Mrqk2.png"
              class="h-14"
              alt="Webflow"
            />
            <span class="dark:text-white">Webflow</span>
          </div>
          <div class="p-1 card-mini">
            <img
              src="https://thumbs.dreamstime.com/b/seo-logo-magnifying-glass-search-engine-optimization-blue-yellow-red-green-color-98240334.jpg"
              class="h-14"
              alt="SEO"
            />
            <span class="dark:text-white">SEO</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
