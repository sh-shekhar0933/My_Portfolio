<template>
  <div class="bg-slate-100 mt-0 shadow-2xl">
    <div
      class="text-xl font-mono flex items-center justify-between h-[80px] px-4 md:px-[200px]"
    >
      <div class="font-bold"><NuxtLink to="/">Shivanshu</NuxtLink></div>
      <button
        @click="toggleNavbar"
        data-collapse-toggle="navbar-default"
        type="button"
        class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200"
        aria-controls="navbar-default"
        aria-expanded="false"
      >
        <span class="sr-only">Open main menu</span>
        <svg
          class="w-5 h-5"
          aria-hidden="true"
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 17 14"
        >
          <path
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M1 1h15M1 7h15M1 13h15"
          />
        </svg>
      </button>
      <div class="hidden md:flex items-center justify-between w-[500px]">
        <ul class="flex items-center">
          <li
            class="hover:bg-sky-200 rounded-lg transition duration-1000 p-2 mx-3"
          >
            <NuxtLink to="/">Home</NuxtLink>
          </li>
          <li
            class="hover:bg-sky-200 rounded-lg transition duration-1000 p-2 mx-3"
          >
            <NuxtLink to="/about">About</NuxtLink>
          </li>
          <li
            class="hover:bg-sky-200 rounded-lg transition duration-1000 p-2 mx-3"
          >
            <NuxtLink to="/skills">Skills</NuxtLink>
          </li>
          <li
            class="hover:bg-sky-200 rounded-lg transition duration-1000 p-2 mx-3"
          >
            <NuxtLink to="/projects">Projects</NuxtLink>
          </li>
          <li
            class="hover:bg-sky-200 transition duration-1000 rounded-lg p-2 mx-3"
          >
            <NuxtLink to="/resume">Resume</NuxtLink>
          </li>
        </ul>
      </div>
    </div>
    <div
      :class="{ hidden: !isNavbarVisible, block: isNavbarVisible }"
      class="md:hidden w-full px-4"
      id="navbar-default"
    >
      <ul class="flex flex-col items-center">
        <li
          class="hover:bg-sky-200 rounded-lg transition duration-1000 p-2 w-full text-center"
        >
          <NuxtLink to="/">Home</NuxtLink>
        </li>
        <li
          class="hover:bg-sky-200 rounded-lg transition duration-1000 p-2 w-full text-center"
        >
          <NuxtLink to="/about">About</NuxtLink>
        </li>
        <li
          class="hover:bg-sky-200 rounded-lg transition duration-1000 p-2 w-full text-center"
        >
          <NuxtLink to="/skills">Skills</NuxtLink>
        </li>
        <li
          class="hover:bg-sky-200 rounded-lg transition duration-1000 p-2 w-full text-center"
        >
          <NuxtLink to="/projects">Projects</NuxtLink>
        </li>
        <li
          class="hover:bg-sky-200 transition duration-1000 rounded-lg p-2 w-full text-center"
        >
          <NuxtLink to="/resume">Resume</NuxtLink>
        </li>
      </ul>
    </div>
    <slot />
  </div>
</template>

<script setup>
import { ref } from "vue";

const isNavbarVisible = ref(false);
const toggleNavbar = () => {
  isNavbarVisible.value = !isNavbarVisible.value;
};
</script>

<style scoped>
/* Add any additional styles if necessary */
</style>
