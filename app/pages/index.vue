<template>
    <h1 class="text-3xl font-bold underline">{{ store.count }}</h1>
    <button @click="increase">Increas</button>
</template>
<script setup>
import { useAuthStore } from '@/stores/auth'

const store = useAuthStore()
const increase = () => {
    store.increment()
}
</script>
<style scoped></style>
