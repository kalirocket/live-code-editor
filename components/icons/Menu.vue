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
    >
    <line x1="4" x2="20" y1="12" y2="12"></line>
    <line x1="4" x2="20" y1="6" y2="6"></line>
    <line x1="4" x2="20" y1="18" y2="18"></line>
  </svg>
</template>
