<template>
  <div class="text-center">
    <div class="">
      <iframe :src="pdfSrc" width="100%" height="600px"></iframe>
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

<script setup>
const pdfSrc = ref("/_nuxt/public/Shivanshu CV 2.pdf");
</script>
