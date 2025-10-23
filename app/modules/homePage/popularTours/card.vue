<template>
  <div
    class="w-full flex rounded-3xl overflow-hidden bg-white"
    style="box-shadow: 0px 4px 12px 3px #0000000D"
  >
    <img
      src="/images/homePage/test.png"
      width="196"
      height="196"
      alt="Logo"
    />

    <div class="p-6 w-full flex flex-col gap-8">
      <div class="flex justify-between items-center">
        <p class="text-2xl font-extrabold text-[#1C1C1F]">
          تور فرانسه + آلمان + سوئیس از مبدا تهران
        </p>
        <div class="text-xl font-medium text-[#1C1C1F] flex items-center gap-2">
          <Clock4 size="24" />
          <p>۱۱ شب و ۱۰ روز</p>
        </div>
      </div>

      <hr class="text-[#E6E6E6] w-full" />

      <div class="flex justify-between items-center">
        <div class="text-xl flex gap-2 items-center font-medium text-[#1C1C1F]">
          <p>از ۲۹٬۹۹۹٬۱۹۰ تومان</p>+<p>۱۷۸۰ دلار</p>
        </div>

        <div class="text-xl flex gap-2 items-center font-medium text-[#1C1C1F]">
          <Calendar />
          <p>ویژه دی و بهمن</p>
        </div>

        <div class="text-xl flex gap-2 items-center font-medium text-[#1C1C1F]">
          <Calendar />
          <p>ایران ایرتور</p>
        </div>

        <NuxtLink
          to=""
          class="text-base py-2 px-5 rounded-3xl font-semibold bg-[#D3AE60] text-white"
        >
          مشاهده تور
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script setup>
import { Calendar, Clock4 } from 'lucide-vue-next'
</script>
