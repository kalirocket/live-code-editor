<script setup lang="ts">
const props = defineProps<{
  type: "file" | "folder";
  name: string;
}>();
</script>
<template>
  <button
    class="ring-offset-background focus-visible:ring-ring hover:text-accent-foreground inline-flex h-10 w-full items-center justify-start gap-2 whitespace-nowrap rounded-md px-2 py-2 text-sm font-medium transition-colors hover:bg-[#333333] focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50"
  >
    <IconsFile v-if="props.type == 'file'" />
    <IconsFolder v-else-if="props.type == 'folder'" />
    <span class="truncate">{{ props.name }}</span>
  </button>
</template>
