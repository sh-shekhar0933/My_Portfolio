<template>
  <div>
    <div
      class="w-[580px] text-md my-5 rounded-t-xl bg-gray-200 h-[68px] px-auto"
    >
      <div class="px-5 py-5">
        <span class="font-bold">{{ props.title }}: </span
        ><span>{{ props.description }}</span>
      </div>
      <div class="w-[580px] h-[4px] bg-gray-900"></div>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  title: {
    type: String,
    required: true,
  },
  description: {
    type: String,
    required: true,
    default: "Default description",
  },
});
</script>
