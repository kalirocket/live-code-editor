<script setup lang="ts">
import type { HTMLAttributes } from "vue";
import { cn } from "@/lib/utils";
import { nanoid } from "nanoid";

interface SkeletonProps {
  class?: HTMLAttributes["class"];
  loading?: boolean;
}

const props = defineProps<SkeletonProps>();

const id = ref<string>("");

onMounted(() => {
  id.value = nanoid();
  setTimeout(() => {
    const element = document.getElementById(id.value);
  }, 0);
});
</script>

<template>
  <div :class="cn('animate-pulse bg-[#27272a]', props.class)" :id="id" />
</template>
