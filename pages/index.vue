<script setup lang="ts">
definePageMeta({
  layout: "home",
});
</script>

<template>
  <div class="flex h-full w-full flex-row">
    <!--  Code section-->
    <!--    <div class="flex h-full w-[60%] flex-col border border-black bg-green-200">-->
    <!--      &lt;!&ndash;    Top header&ndash;&gt;-->
    <!--      <div-->
    <!--        class="bg-headerBg text-headerText font-lato flex h-auto w-full flex-row items-center justify-between px-5 py-3"-->
    <!--      >-->
    <!--        &lt;!&ndash;      Some actions here&ndash;&gt;-->
    <!--        <div class="flex flex-row items-center gap-x-4">-->
    <!--          <IconsMaterialSymbolsMenu />-->
    <!--          <div class="flex flex-row items-center gap-x-1">-->
    <!--            <div>File</div>-->
    <!--            <IconsMaterialSymbolsArrowDropDown />-->
    <!--          </div>-->
    <!--          <div class="flex flex-row items-center gap-x-1">-->
    <!--            <div>Edit</div>-->
    <!--            <IconsMaterialSymbolsArrowDropDown />-->
    <!--          </div>-->
    <!--          <div class="flex flex-row items-center gap-x-1">-->
    <!--            <div>View</div>-->
    <!--            <IconsMaterialSymbolsArrowDropDown />-->
    <!--          </div>-->
    <!--        </div>-->
    <!--        &lt;!&ndash;      Some other actions here&ndash;&gt;-->
    <!--        <div class="flex flex-row items-center gap-x-4">-->
    <!--          <IconsMaterialSymbolsSearch />-->
    <!--          <IconsMaterialSymbolsSettings />-->
    <!--          <IconsMaterialSymbolsAccountCircle />-->
    <!--        </div>-->
    <!--      </div>-->
    <!--      &lt;!&ndash;    Code editor&ndash;&gt;-->
    <!--      <div class="flex h-full w-full flex-row">-->
    <!--        &lt;!&ndash;      File/Folder Explorer&ndash;&gt;-->
    <!--        <div class="h-full w-[40%] bg-red-200"></div>-->
    <!--        &lt;!&ndash;      Actual Code&ndash;&gt;-->
    <!--        <div class="h-full w-[60%] bg-gray-300"></div>-->
    <!--      </div>-->
    <!--      &lt;!&ndash;    Bottom footer&ndash;&gt;-->
    <!--      <div class="flex h-auto w-full flex-row items-center justify-between">-->
    <!--        <div class="flex flex-row items-center">-->
    <!--          <div class="flex items-center">-->
    <!--            <IconsMaterialSymbolsPowerSettingsNew />-->
    <!--            <div>Typescript</div>-->
    <!--          </div>-->
    <!--          <div class="flex items-center">-->
    <!--            <IconsSelector />-->
    <!--            <div>1,234 lines</div>-->
    <!--          </div>-->
    <!--          <div class="flex items-center">-->
    <!--            <IconsCarbonDebug />-->
    <!--            <div>0 errors</div>-->
    <!--          </div>-->
    <!--        </div>-->
    <!--        <div class="flex flex-row items-center">-->
    <!--          <div class="flex items-center">-->
    <!--            <IconsMaterialSymbolsLightNestClockFarsightAnalogOutline />-->
    <!--            <div>12:34 PM</div>-->
    <!--          </div>-->
    <!--        </div>-->
    <!--      </div>-->
    <!--    </div>-->
    <InterfaceCodeEditor />
    <!--  Preview/Output section-->
    <div
      class="h-full w-[40%] border border-y-black border-r-black bg-yellow-200"
    ></div>
  </div>
</template>
