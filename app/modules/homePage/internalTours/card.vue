<template>
  <div
    class="w-full rounded-3xl relative bg-white"
    style="box-shadow: 0px 4px 9px 3px #0000001C"
  >
    <img
      src="/images/homePage/test.png"
      width="300"
      height="300"
      alt="Logo"
      class="w-full rounded-t-3xl"
    />
    <img
      src="/images/homePage/internalSvg.png"
      width="91"
      height="91"
      alt="discount"
      class="absolute top-0 right-4 translate-x-1/2 -translate-y-1/2"
    />

    <div class="py-6 px-3 flex flex-col gap-6">
      <div class="flex justify-between items-center">
        <p class="text-2xl font-extrabold text-[#1C1C1F]">زمینی وان</p>
        <p class="text-xl font-medium text-[#1C1C1F]">اسفند</p>
      </div>
      <div class="flex justify-between items-center">
        <p class="text-xl font-medium text-[#1C1C1F]">از ۲۹٬۹۹۹٬۱۹۰ تومان</p>
        <NuxtLink
          to=""
          class="text-base py-2 px-5 rounded-3xl font-semibold bg-[#511424] text-white"
        >
          مشاهده
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script setup>
</script>
