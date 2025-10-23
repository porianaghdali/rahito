<template>
  <div class="w-full">
    <div class="flex flex-col items-center relative mb-2">
      <img
        src="/images/homePage/vector.png"
        class="absolute top-[50%] left-[50%] -translate-x-1/2 -translate-y-1/2"
        width="420"
        height="200"
        alt="Logo"
      />
      <p class="font-extrabold text-[32px] text-[#1C1C1F] z-20">مقاصد برگزیده</p>
    </div>

    <p class="text-base font-medium text-[#1C1C1F] text-center mb-12">
      مقاصد پرطرفدار انتخاب شده توسط مسافران تور‌های زمستان-بهار
    </p>

    <div class="flex gap-6 justify-center">
      <Card />
      <Card />
      <Card />
      <Card />
    </div>
  </div>
</template>

<script setup>
import Card from './Card.vue'
</script>
