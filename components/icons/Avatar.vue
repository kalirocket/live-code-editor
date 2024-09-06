<script setup lang="ts">
const props = defineProps<{
  src?: string;
  alt?: string;
  size?: "sm" | "md" | "lg";
  type?: "icon" | "image";
}>();

let height: string, width: string;

switch (props.size) {
  case "sm":
    height = "12";
    width = "12";
    break;
  case "md":
    height = "16";
    width = "16";
    break;
  case "lg":
    height = "20";
    width = "20";
    break;
}
</script>

<template>
  <img
    v-if="props.type !== 'icon'"
    :class="{
      'h-[24px] w-[24px]': props.size === 'sm',
      'h-[32px] w-[32px]': props.size === 'md',
      'h-[40px] w-[40px]': props.size === 'lg',
    }"
    class="ring-avatar-border rounded-full object-cover p-[2px] ring-2"
    :src="src"
    :alt="props.alt"
  />
  <div
    v-if="props.type == 'icon'"
    :class="{
      'h-[24px] w-[24px]': props.size === 'sm',
      'h-[32px] w-[32px]': props.size === 'md',
      'h-[40px] w-[40px]': props.size === 'lg',
    }"
    class="ring-avatar-border flex items-center justify-center rounded-full object-cover ring-2"
  >
    <User stroke="avatar-user" :height="height" :width="width" />
  </div>
</template>
