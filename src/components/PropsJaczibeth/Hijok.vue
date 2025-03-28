<script setup>
import { ref } from 'vue'

defineProps({
 edad: String,
})
</script>

<template>

<p> Tengo la edad de:{{ edad }}</p>
</template>

<style scoped></style>