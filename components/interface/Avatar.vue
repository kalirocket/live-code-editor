<script setup lang="ts">
const props = defineProps<{
  src?: string;
  alt?: string;
  size?: "sm" | "md" | "lg";
  class?: string;
}>();

let size: string;

switch (props.size) {
  case "sm":
    size = "h-7 w-7";
    break;
  case "md":
    size = "h-10 w-10";
    break;
  case "lg":
    size = "h-15 w-15";
    break;
  default:
    size = "h-7 w-7";
}

const full_class = `ring-gray-300 rounded-full object-cover p-1 ring-1 ${size} ${props.class}`;
</script>
<template>
  <img v-if="src" :class="full_class" :src="props.src" :alt="props.alt" />
  <div v-else class="flex items-center justify-center" :class="full_class">
    <slot />
  </div>
</template>
