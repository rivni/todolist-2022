<script setup>
import  { ref, computed } from "vue";

const count = ref(0);
const countMessage = computed(() => "回数: " + count.value);
</script>

<template>
    <div>{{ countMessage }}</div>
    <button @click="count++">クリック！</button>
    <button @click="count = count * count">押すな！</button>
    <button @click="count = 0">リセット！</button>
</template>

<style></style>