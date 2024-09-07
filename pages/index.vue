<script setup lang="ts">
definePageMeta({
  layout: "home",
});
</script>

<template>
  <div class="flex h-full w-full flex-row">
    <InterfaceCodeEditor />
    <!--  Preview/Output section-->
    <div
      class="h-full w-[40%] border border-y-black border-r-black bg-yellow-200"
    ></div>
  </div>
</template>
