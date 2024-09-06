<script setup lang="ts">
const props = defineProps<{
  fill?: string;
  stroke?: string;
  width?: string;
  height?: string;
  strokeWidth?: string;
  class?: string;
}>();
</script>

<template>
  <svg
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 24 24"
    fill="none"
    :stroke="stroke ?? 'currentColor'"
    :stroke-width="strokeWidth ?? 2"
    stroke-linecap="round"
    stroke-linejoin="round"
    class="h-5 w-5"
    :class="props.class"
  >
    <path d="M12 2v10"></path>
    <path d="M18.4 6.6a9 9 0 1 1-12.77.04"></path>
  </svg>
</template>
