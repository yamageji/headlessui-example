<template>
  <div class="py-[24px] px-[12px] md:px-[30px] bg-gray-200 w-full min-h-full">
    <h2 class="text-[30px] font-bold text-gray-700">Headless UI samples</h2>

    <div class="grid grid-cols-2 auto-rows-auto gap-[24px]">
      <div
        class="
          col-span-2
          mt-[24px]
          bg-yellow-500
          px-[24px]
          pt-[18px]
          pb-[18px]
          rounded-md
        "
      >
        <div class="flex max-w-xl mx-auto">
          <h2 class="text-2xl font-bold text-yellow-100">Dialog</h2>
          <div class="ml-[36px]">
            <BasicDialog />
          </div>
          <div class="ml-[12px]">
            <TransitionDialog />
          </div>
        </div>
      </div>

      <div
        class="col-span-2 bg-green-500 px-[24px] pt-[18px] pb-[30px] rounded-md"
      >
        <div class="max-w-xl mx-auto">
          <h2 class="text-2xl font-bold text-green-100">Tabs</h2>
          <div class="mt-[18px]">
            <BasicTabs />
          </div>
        </div>
      </div>

      <div
        class="
          col-span-2
          bg-indigo-500
          px-[24px]
          pt-[18px]
          pb-[30px]
          rounded-md
        "
      >
        <div class="max-w-xl mx-auto">
          <h2 class="text-2xl font-bold text-indigo-100">Disclosure</h2>
          <div class="flex gap-[24px] mt-[18px]">
            <BasicDisclosure />
            <TransitionDisclosure />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import BasicDialog from '../components/BasicDialog.vue';
import BasicDisclosure from '../components/BasicDisclosure.vue';
import BasicTabs from '../components/BasicTabs.vue';
import TransitionDialog from '../components/TransitionDialog.vue';
import TransitionDisclosure from '../components/TransitionDisclosure.vue';
export default defineComponent({
  components: {
    BasicDialog,
    BasicDisclosure,
    BasicTabs,
    TransitionDialog,
    TransitionDisclosure,
  },
});
</script>
