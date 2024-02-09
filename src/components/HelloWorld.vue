<script setup>
import { ref } from 'vue'
import { valPlusOne } from '@/utils/';

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button type="button" @click="count++">count is {{ count }} and is not {{ valPlusOne(count) }}</button>
  </div>
</template>

<style scoped>

</style>
