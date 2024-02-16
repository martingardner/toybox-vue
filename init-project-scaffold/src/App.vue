<script setup>
  import { ref } from 'vue'
  import ObjectCount from './components/ObjectCount.vue';
  import ObjectBtnTrigger from './components/ObjectBtnTrigger.vue';
  import ComposableBtnTrigger from './components/ComposableBtnTrigger.vue';
  const count = ref(0)
</script>


<template>
  <main>
    <button @click="count++">Count is: {{ count }}</button>
    <ObjectCount />
    <ObjectBtnTrigger />
    <ComposableBtnTrigger />
  </main>
</template>

<style scoped>
button {
  font-weight: bold
}
</style>
