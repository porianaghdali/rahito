<template>
  <div class="relative group grid">
    <!-- کارت اصلی -->
    <div
      class="w-full flex flex-col gap-8 rounded-3xl py-12 z-10 relative transition-all duration-300 hover:bg-white hover:shadow-[0px_4px_9px_3px_#0000001C]"
    >
      <img :src="src" width="144" height="144" alt="Logo" class="mx-auto" />

      <div class="flex flex-col gap-6 px-6">
        <div class="flex justify-center items-center">
          <p class="text-2xl font-extrabold text-[#1C1C1F] text-center">
            {{ title }}
          </p>
        </div>
        <div class="flex justify-center items-center">
          <p class="text-xl font-medium text-[#1C1C1F] leading-8 text-center">
            {{ description }}
          </p>
        </div>
      </div>
    </div>

    <!-- تصویر وکتور (زیر کارت) -->
    <img
      src="/images/homePage/RahitoVsOthers/vector.png"
      width="86"
      height="86"
      alt="vector"
      class="mx-auto absolute bottom-0 left-0 -translate-x-1/2 translate-y-1/2 z-0 opacity-0 group-hover:opacity-100"
    />
  </div>
</template>

<script setup>
defineProps({
  title: String,
  description: String,
  src: String
})
</script>
