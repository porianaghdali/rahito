<script setup>
import { CircleUserRound } from 'lucide-vue-next'

const list = [
  { title: 'خانه', id: 'home' },
  { title: 'تورهای مسافرتی', id: 'tours' },
  { title: 'هتل‌ها', id: 'hotels' },
  { title: 'ویزا', id: 'visa' },
  { title: 'سفرنامه', id: 'blog' },
  { title: 'تماس با ما', id: 'contantUs' }
]
</script>

<template>
  <header class="flex justify-between mb-16 px-[7%] pt-[3%]">
    <!-- Logo -->
    <NuxtLink to="/">
      <img src="/images/logo.png" width="150" height="44" alt="Logo" />
    </NuxtLink>

    <!-- Navigation -->
    <ul class="flex gap-10">
      <li
        v-for="item in list"
        :key="item.id"
        class="font-bold text-xl rounded-3xl p-3 hover:bg-[#D3AE60] hover:text-white transition-colors duration-200"
      >
        <NuxtLink :to="`/${item.id}`">{{ item.title }}</NuxtLink>
      </li>
    </ul>

    <!-- Login / Register -->
    <NuxtLink
      to="/sign-up"
      class="flex gap-2 items-center py-2.5 pr-6 pl-4 rounded-3xl bg-[#1C1C1F] hover:bg-[#333]"
    >
      <span class="text-white">ورود/ثبت‌نام</span>
      <CircleUserRound color="white" />
    </NuxtLink>
  </header>
</template>
