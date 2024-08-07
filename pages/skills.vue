<template>
  <div>
    <div
      class="lg:flex lg:items-center lg:justify-between lg:mx-[200px] sm:mx-[100px] my-[52px] onfade"
    >
      <div>
        <h1 class="text-3xl font-bold text-gray-600">
          Professional Skills and Knowledge
        </h1>
        <ul class="text-md mt-[20px]">
          <li class="my-[32px]">
            <skill
              title="Front End Web Development"
              description="HTML ,CSS ,JavaScript ,ReactJS ,VueJs ,Nuxt3"
            ></skill>
          </li>
          <li class="my-[32px]">
            <skill
              title="Tools"
              description="Visual Studio Code ,Github  "
            ></skill>
          </li>
          <li class="my-[32px]">
            <skill
              title="Problem Solving"
              description=" Data Stuctures and Algorithms in C++  "
            ></skill>
          </li>
          <li class="my-[32px]">
            <skill
              title="CS fundamentals "
              description=" OOPS,Operating Systems ,DBMS ,Computer Networks "
            ></skill>
          </li>
        </ul>
      </div>

      <div class="w-[500px] my-[80px]">
        <img
          class="h-[320px] mt-[40px] rounded-lg"
          src="/public/SKills.jpg"
          alt=""
        />
      </div>
    </div>

    <div class="mb-0 ml-0 mr-0 bg-slate-600 text-center p-5">
      <h1 class="text-white text-4xl font-bold">Thank you</h1>
      <a class="inline-block" href=""
        ><img
          class="h-[32px] w-[32px] mr-5 mt-[32px]"
          src="/public/facebook.png"
          alt=""
      /></a>
      <a class="inline-block" href=""
        ><img
          class="h-[32px] w-[32px] mr-5 mt-[32px]"
          src="/public/social.png"
          alt=""
      /></a>
      <p class="text-white text-md mt-[40px]">
        &copy;2024 Copyright all rights reserved
      </p>
    </div>
  </div>
</template>
