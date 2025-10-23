<script setup>
import HeroSection from '../modules/homePage/heroSection/heroSection.vue'
import ChosenDestinations from '../modules/homePage/chosenDestinations/chosenDestinations.vue'
import SearchSection from '../modules/homePage/searchSection/searchSection.vue'
import PopularTours from '../modules/homePage/popularTours/popularTours.vue'
import InternalTours from '../modules/homePage/internalTours/internalTours.vue'
import RahitoVsOthers from '../modules/homePage/rahitoVsOthers/rahitoVsOthers.vue'
import Blogs from '../modules/homePage/blogs/blogs.vue'
import AboutTour from '../modules/homePage/aboutTour/aboutTour.vue'
import SignUp from '../modules/homePage/signUp/signUp.vue'
</script>

<template dir="rtl">
  <div class="px-[5%]">
    <div class="mb-16">
      <HeroSection />
    </div>

    <div class="flex flex-col gap-32 mb-30">
      <SearchSection />
      <ChosenDestinations />
      <PopularTours />
      <InternalTours />
      <RahitoVsOthers />
      <Blogs />
      <AboutTour />
      <SignUp />
    </div>
  </div>
</template>
