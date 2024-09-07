<script setup lang="ts">
import { Splitpanes, Pane } from "splitpanes";
import "splitpanes/dist/splitpanes.css";
</script>
<template>
  <div class="flex h-full w-full flex-col bg-[#1e1e1e] text-[#d4d4d4]">
    <!--    header-->
    <header
      class="flex h-12 shrink-0 items-center border-b border-[#333333] px-4"
    >
      <nav class="flex items-center gap-4">
        <InterfaceActionButton>
          <IconsMenu />
        </InterfaceActionButton>
      </nav>
      <div class="ml-auto flex items-center gap-2">
        <InterfaceActionButton>
          <IconsSearch />
        </InterfaceActionButton>
        <InterfaceActionButton>
          <IconsSettings />
        </InterfaceActionButton>
        <InterfaceAvatar
          src="https://avatars.githubusercontent.com/u/61436567?v=4"
        >
          <IconsMaterialSymbolsAccountCircle class="h-full w-full" />
        </InterfaceAvatar>
      </div>
    </header>
    <!--    main content-->
    <div class="flex flex-1">
      <splitpanes style="height: 100%; width: 100%">
        <pane size="30%">
          <div
            class="h-full w-full shrink-0 overflow-auto border-r border-[#333333] bg-[#252526]"
          >
            <div class="p-4">
              <div class="mb-4 flex items-center gap-2 text-sm">
                <IconsFolder />
                <span class="font-medium">Project</span>
              </div>
              <div class="grid gap-2">
                <InterfaceFileFolderButton type="file" name="index.html" />
                <InterfaceFileFolderButton type="file" name="index.js" />
                <InterfaceFileFolderButton type="file" name="style.css" />
              </div>
            </div>
          </div>
        </pane>
        <pane size="100%">
          <div class="h-full w-full flex-1 overflow-auto">
            <div class="relative h-full">
              <div
                class="absolute inset-0 bg-[#1e1e1e] p-4 font-mono text-sm leading-6 text-[#d4d4d4]"
              >
                <div class="grid gap-2">
                  <div class="flex items-center gap-2">
                    <div class="w-6 text-right text-[#6a6a6a]">1</div>
                    <div class="flex-1">
                      <span class="text-[#569cd6]">import</span>
                      <span class="text-[#9cdcfe]">React</span>{" "}
                      <span class="text-[#569cd6]">from</span>
                      <span class="text-[#ce9178]">'react'</span>;
                    </div>
                  </div>
                  <div class="flex items-center gap-2">
                    <div class="w-6 text-right text-[#6a6a6a]">2</div>
                    <div class="flex-1">
                      <span class="text-[#569cd6]">import</span>
                      <span class="text-[#9cdcfe]">ReactDOM</span>{" "}
                      <span class="text-[#569cd6]">from</span>
                      <span class="text-[#ce9178]">'react-dom'</span>;
                    </div>
                  </div>
                  <div class="flex items-center gap-2">
                    <div class="w-6 text-right text-[#6a6a6a]">3</div>
                    <div class="flex-1">
                      <span class="text-[#569cd6]">import</span>
                      <span class="text-[#9cdcfe]">App</span>{" "}
                      <span class="text-[#569cd6]">from</span>
                      <span class="text-[#ce9178]">'./App'</span>;
                    </div>
                  </div>
                  <div class="flex items-center gap-2">
                    <div class="w-6 text-right text-[#6a6a6a]">4</div>
                    <div class="flex-1">
                      <span class="text-[#569cd6]">import</span>
                      <span class="text-[#9cdcfe]">styles</span>{" "}
                      <span class="text-[#569cd6]">from</span>
                      <span class="text-[#ce9178]">'./styles.css'</span>;
                    </div>
                  </div>
                  <div class="flex items-center gap-2">
                    <div class="w-6 text-right text-[#6a6a6a]">5</div>
                    <div class="flex-1">
                      <span class="text-[#569cd6]">ReactDOM</span>
                      <span class="text-[#d4d4d4]">.</span>
                      <span class="text-[#9cdcfe]">render</span>
                      <span class="text-[#d4d4d4]">(</span>
                      <span class="text-[#9cdcfe]">
                        <span class="text-[#d4d4d4]">&lt;</span>App<span
                          class="text-[#d4d4d4]"
                          >/&gt;</span
                        >
                      </span>
                      <span class="text-[#d4d4d4]">)</span>
                      <span class="text-[#d4d4d4]">;</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </pane>
      </splitpanes>
    </div>
    <!--    footer-->
    <div
      class="flex h-8 items-center border-t border-[#333333] bg-[#252526] px-4 text-sm text-[#6a6a6a]"
    >
      <div class="flex items-center gap-2">
        <IconsPowerSwitch />
        <span>TypeScript</span>
      </div>
      <div class="ml-4 flex items-center gap-2">
        <IconsArrowLeftRight />
        <span>1,234 lines</span>
      </div>
      <div class="ml-4 flex items-center gap-2">
        <IconsDebug />
        <span>0 errors</span>
      </div>
      <div class="ml-auto flex items-center gap-2">
        <IconsClock />
        <span>12:34 PM</span>
      </div>
    </div>
  </div>
</template>
<style>
.splitpanes--vertical > .splitpanes__splitter {
  min-width: 20px;
  margin-left: -10px;
}

.splitpanes--horizontal > .splitpanes__splitter {
  min-width: 20px;
}
</style>
