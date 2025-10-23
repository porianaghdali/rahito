<template>
  <div class="w-full">
    <div class="flex justify-center relative mb-4 gap-2">
      <img
        src="/images/homePage/intenalTitle.png"
        width="30"
        height="46"
        alt="discount"
      />
      <p class="font-extrabold text-[32px] text-[#1C1C1F]">تورهای داخلی</p>
    </div>

    <p class="text-base font-medium text-[#1C1C1F] text-center mb-12">
      تورهای ویژه ارزان قیمت و زمینی
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
