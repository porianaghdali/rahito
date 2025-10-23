<template>
  <div class="w-full">
    <div class="flex flex-col items-center relative mb-2">
      <p class="font-extrabold text-[32px] text-[#1C1C1F] z-20">تورهای پرطرفدار</p>
    </div>

    <p class="text-base font-medium text-[#1C1C1F] text-center mb-12">
      تورهای ویژه فصل و تعطیلات مهم پیش‌رو
    </p>

    <div class="flex flex-col gap-6">
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
