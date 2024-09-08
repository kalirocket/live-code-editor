<script setup lang="ts">
definePageMeta({
  layout: "home",
});
</script>

<template>
  <div class="flex h-full w-full flex-row">
    <InterfaceCodeEditor />
    <!--  Preview/Output section-->
    <InterfaceSkeleton
      class="h-full w-[40%] border-y border-r border-black"
    ></InterfaceSkeleton>
  </div>
</template>
