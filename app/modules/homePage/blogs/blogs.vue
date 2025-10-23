<template>
  <div class="w-full">
    <div class="flex flex-col items-center relative mb-2">
      <p class="font-extrabold text-[32px] text-[#1C1C1F] z-20">
        سفرنامه‌ها و مجله گردشگری
      </p>
    </div>

    <p class="text-base font-medium text-[#1C1C1F] text-center mb-12">
      هرچه راجب سفر نیاز دارید، را بخوانید
    </p>

    <div class="flex gap-6 justify-center">
      <!-- بلاگ بزرگ سمت چپ -->
      <div
        class="w-[38%] h-fit rounded-3xl bg-white shadow-[0px_4px_9px_3px_#0000001C]"
      >
        <div
          class="col-span-1 h-[340px] w-full px-6 py-4 rounded-3xl bg-center bg-cover grid items-end"
          style="background-image: url('/images/homePage/blog.png')"
        >
          <div
            style="backdrop-filter: blur(12px)"
            class="font-semibold text-base py-2 text-center mt-auto rounded-3xl bg-white/40 text-white"
          >
            بیشتر بخوانید
          </div>
        </div>

        <div class="p-6">
          <p class="font-bold text-2xl leading-8 text-[#212121]">
            چه مواردی را برای سفر به مسکو در تابستان بدانیم؟
          </p>
          <div class="flex justify-between items-center mt-2">
            <p>۱۴۰۴/۰۲/۱۷</p>
            <div class="flex gap-1 items-center">
              <Icon name="lucide:clock-4" size="24" />
              <p>زمان مطالعه: ۵ دقیقه</p>
            </div>
          </div>
        </div>
      </div>

      <!-- دو کارت سمت راست -->
      <div class="grid gap-6 w-[62%]">
        <Card />
        <Card />
      </div>
    </div>
  </div>
</template>

<script setup>
import Card from './Card.vue'

</script>
