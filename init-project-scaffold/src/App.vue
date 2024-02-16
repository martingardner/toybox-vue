<script setup>
  import { ref } from 'vue'
  import ObjectCount from './components/ObjectCount.vue';
  const count = ref(0)
</script>


<template>
  <main>
    <button @click="count++">Count is: {{ count }}</button>
    <ObjectCount />
  </main>
</template>

<style scoped>
button {
  font-weight: bold
}
</style>
