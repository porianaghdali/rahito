<script setup>
import { Twitter, Instagram, Facebook } from 'lucide-vue-next'

const links = [
  { title: 'تورهای داخلی', id: 'Domestic Tours' },
  { title: 'تورهای خارجی', id: 'Foreign tours' },
  { title: 'لیست هتل‌ها', id: 'hotels' },
  { title: 'مقاصد پرطرفدار', id: 'Popular destinations' }
]

const moreLinks = [
  { title: 'ویزای توریستی', id: 'Tourist visa' },
  { title: 'دانستنی‌های سفر', id: 'Travel information' },
  { title: 'باشگاه مشتریان', id: 'Customer club' },
  { title: 'سفرنامه', id: 'blogs' }
]

const contactUs = [
  { title: 'پشتیبانی', id: 'Support' },
  { title: 'سوالات متداول', id: 'faq' },
  { title: 'اطلاعات تماس', id: 'Contact information' },
  { title: 'همکاری با ما', id: 'Cooperate with us' }
]
</script>

<template>
  <footer>
    <div class="grid grid-cols-2 justify-between px-[5%] mb-8 pb-8 pt-[3%] border-b border-[#9999998F]">
      <div class="max-w-[241px]">
        <img src="/images/logo.png" width="150" height="44" alt="Logo" class="mb-2" />
        <p class="font-medium text-sm text-[#1C1C1F] mb-3 pb-4">
          رزرو تور های مسافرتی خارجی و داخلی با لیستی از بهترین هتل‌ها و اقامتگاه‌ها
        </p>
        <div class="flex gap-5">
          <button
            class="bg-white p-4 shadow-[0px_1.83px_9.15px_0px_#0000001A] w-fit rounded-full text-[#444444] hover:bg-[#511424] hover:text-white"
          >
            <Twitter />
          </button>
          <button
            class="bg-white p-4 shadow-[0px_1.83px_9.15px_0px_#0000001A] w-fit rounded-full text-[#444444] hover:bg-[#511424] hover:text-white"
          >
            <Instagram />
          </button>
          <button
            class="bg-white p-4 shadow-[0px_1.83px_9.15px_0px_#0000001A] w-fit rounded-full text-[#444444] hover:bg-[#511424] hover:text-white"
          >
            <Facebook />
          </button>
        </div>
      </div>

      <div class="flex justify-between">
        <div class="flex flex-col gap-8">
          <p class="font-semibold text-xl text-[#222222]">لینک ها اصلی</p>
          <div class="grid gap-4">
            <NuxtLink
              v-for="item in links"
              :key="item.id"
              to="/"
              class="text-[#666666] font-normal text-base"
            >
              {{ item.title }}
            </NuxtLink>
          </div>
        </div>

        <div class="flex flex-col gap-8">
          <p class="font-semibold text-xl text-[#222222]">تماس با ما</p>
          <div class="grid gap-4">
            <NuxtLink
              v-for="item in contactUs"
              :key="item.id"
              to="/"
              class="text-[#666666] font-normal text-base"
            >
              {{ item.title }}
            </NuxtLink>
          </div>
        </div>

        <div class="flex flex-col gap-8">
          <p class="font-semibold text-xl text-[#222222]">لینک های بیشتر</p>
          <div class="grid gap-4">
            <NuxtLink
              v-for="item in moreLinks"
              :key="item.id"
              to="/"
              class="text-[#666666] font-normal text-base"
            >
              {{ item.title }}
            </NuxtLink>
          </div>
        </div>
      </div>
    </div>

    <div class="px-[5%] flex justify-between mb-16">
      <p class="text-[#666666] text-sm font-medium">قوانین و مقررات استفاده</p>
      <p class="text-[#666666] text-sm font-medium">
        حق کپی رایت، محفوظ به راهیتو است.
      </p>
    </div>
  </footer>
</template>
