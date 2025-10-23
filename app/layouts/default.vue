<script setup>
import Footer from "../composable/Footer.vue";
import Header from "../composable/Header.vue";
</script>

<template>
  <div dir="rtl">
    <Header/>
    <slot />
    <Footer />
  </div>
  
</template>
