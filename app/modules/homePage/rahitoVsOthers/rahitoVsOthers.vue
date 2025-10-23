<template>
  <div class="w-full">
    <div class="flex flex-col items-center relative mb-4">
      <p class="font-extrabold text-[32px] text-[#1C1C1F]">
        وجه تمایز راهیتو از دیگران
      </p>
    </div>

    <p class="text-base font-medium text-[#1C1C1F] text-center mb-12">
      مقاصد پرطرفدار انتخاب شده توسط مسافران تور‌های زمستان-بهار
    </p>

    <div class="grid grid-cols-4 gap-6 justify-center">
      <Card
        v-for="(item, index) in list"
        :key="index"
        :title="item.title"
        :description="item.description"
        :src="item.src"
      />
    </div>
  </div>
</template>

<script setup>
import Card from './Card.vue'

const list = [
  {
    title: "باشگاه مشتریان",
    description: "باشگاه مشتریان؛ جمع‌آوری امتیاز و دریافت تخفیف‌های ویژه سفر",
    src: "/images/homePage/RahitoVsOthers/customerClub.png",
  },
  {
    title: "پشتیبانی شبانه‌روزی",
    description: "هر روز هفته، ۲۴ ساعته حتی در ایام تعطیل. در تمامی مراحل سفر!",
    src: "/images/homePage/RahitoVsOthers/support.png",
  },
  {
    title: "دستیار هوشمند",
    description: "انتخاب بودجه و مقصد، دریافت پیشنهادات هوشمند تور با اطلاع‌رسانی لحظه‌ای",
    src: "/images/homePage/RahitoVsOthers/ai-Assist.png",
  },
  {
    title: "رزرو گروهی دوستان",
    description: "رزرو گروهی؛ سفر با دوستان، محاسبه هزینه و پرداخت جداگانه!",
    src: "/images/homePage/RahitoVsOthers/group.png",
  },
]
</script>
