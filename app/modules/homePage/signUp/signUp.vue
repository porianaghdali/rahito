<template>
  <div class="bg-[#511424] relative rounded-3xl py-16 flex justify-center items-center">
    <!-- متن و فرم ثبت نام -->
    <div class="max-w-[677px] flex flex-col gap-16 justify-center items-center z-20">
      <p class="font-bold text-[44px] text-white text-center">
        ثبت‌نام برای دریافت آفر های ویژه و <br /> لحظه آخری!
      </p>

      <div class="bg-white rounded-3xl p-3 flex gap-2 items-center w-full">
        <MailIcon class="text-[#999999] w-6 h-6" />
        <input
          type="text"
          placeholder="ایمیل خود را وارد کنید"
          class="flex-1 outline-none px-4 py-2 rounded-3xl"
        />
        <button class="bg-[#511424] py-3 px-4 rounded-3xl text-white">
          ثبت ایمیل
        </button>
      </div>
    </div>

    <!-- تصاویر موقعیت‌یابی شده -->
    <img
      src="/images/homePage/signUp/Element.png"
      alt="Element"
      class="absolute top-0 right-0 w-[121px] h-[108px]"
    />
    <img
      src="/images/homePage/signUp/Group.png"
      alt="Group"
      class="absolute left-0 bottom-0 w-[372px] h-[372px]"
    />
  </div>
</template>

<script setup lang="ts">
import { MailIcon } from "lucide-vue-next"; // معادل Lucide در Vue
</script>
