<script setup>
import { ref } from "vue";
import { Calendar, MapPinIcon, Search, UserRound } from "lucide-vue-next";

const list = [
  { title: "تورهای داخلی", id: "internal" },
  { title: "تورهای خارجی", id: "external" },
  { title: "پرواز", id: "flight" },
  { title: "قطار", id: "train" },
  { title: "اتوبوس", id: "bus" },
  { title: "هتل", id: "hotel" },
];

const details = [
  { title: "مبدا", id: "start", selected: "تهران", icon: MapPinIcon },
  { title: "مقصد", id: "end", selected: "استانبول", icon: MapPinIcon },
  { title: "تاریخ رفت", id: "goneDate", selected: "۱۴۰۴/۰۲/۱۱", icon: Calendar },
  { title: "تاریخ برگشت", id: "returnDate", selected: "۱۴۰۴/۰۲/۱۷", icon: Calendar },
  { title: "تعداد مسافر", id: "numberOfPassengers", selected: "۳", icon: UserRound },
];

const selected = ref("internal");
</script>

<template>
  <div class="mx-auto w-full">
    <div class="bg-white rounded-3xl" style="box-shadow: 0px 4px 9px 3px #0000001C;">
      <ul class="flex">
        <li
          v-for="item in list"
          :key="item.id"
          :class="[
            selected === item.id
              ? 'bg-[#FDFBF7] border-0 rounded-t-3xl text-[#511424]'
              : 'border-b border-[#E6E6E6] text-[#939393]',
            'py-4 px-6'
          ]"
        >
          <button
            class="cursor-pointer font-extrabold text-sm whitespace-nowrap"
            @click="selected = item.id"
          >
            {{ item.title }}
          </button>
        </li>
        <li class="w-full border-b border-[#E6E6E6]"></li>
      </ul>

      <div
        class="w-full flex justify-between p-6 items-center bg-[#FDFBF7] shadow-[0px_4px_9px_3px_rgba(0,0,0,0.11)] rounded-b-3xl"
      >
        <div class="flex flex-col gap-5">
          <div class="flex gap-1 text-[#525252]">
            <MapPinIcon size="24" />
            <p class="text-base font-semibold items-center">مبدا</p>
          </div>
          <div class="text-xl font-semibold text-[#1C1C1F]">تهران</div>
        </div>

        <hr class="w-[1px] h-12 bg-[#E6E6E6]" />

        <div class="flex flex-col gap-5">
          <div class="flex gap-1 text-[#525252]">
            <MapPinIcon size="24" />
            <p class="text-base font-semibold items-center">مقصد</p>
          </div>
          <div class="text-xl font-semibold text-[#1C1C1F]">استانبول</div>
        </div>

        <hr class="w-[1px] h-12 bg-[#E6E6E6]" />

        <div class="flex flex-col gap-5">
          <div class="flex gap-1 text-[#525252]">
            <Calendar size="24" />
            <p class="text-base font-semibold items-center">تاریخ رفت</p>
          </div>
          <div class="text-xl font-semibold text-[#1C1C1F]">۱۴۰۴/۰۲/۱۱</div>
        </div>

        <hr class="w-[1px] h-12 bg-[#E6E6E6]" />

        <div class="flex flex-col gap-5">
          <div class="flex gap-1 text-[#525252]">
            <Calendar size="24" />
            <p class="text-base font-semibold items-center">تاریخ برگشت</p>
          </div>
          <div class="text-xl font-semibold text-[#1C1C1F]">۱۴۰۴/۰۲/۱۷</div>
        </div>

        <hr class="w-[1px] h-12 bg-[#E6E6E6]" />

        <div class="flex flex-col gap-5">
          <div class="flex gap-1 text-[#525252]">
            <UserRound />
            <p class="text-base font-semibold items-center">تعداد مسافر</p>
          </div>
          <div class="text-xl font-semibold text-[#1C1C1F]">۳ نفر</div>
        </div>

        <hr class="w-[1px] h-12 bg-[#E6E6E6]" />

        <div>
          <button class="text-white bg-[#511424] flex items-center gap-2 py-2.5 px-6 rounded-3xl">
            جستجو
            <Search size="18" />
          </button>
        </div>
      </div>
    </div>
  </div>
</template>
