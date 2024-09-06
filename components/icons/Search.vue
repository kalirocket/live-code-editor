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
    <circle cx="11" cy="11" r="8"></circle>
    <path d="m21 21-4.3-4.3"></path>
  </svg>
</template>
