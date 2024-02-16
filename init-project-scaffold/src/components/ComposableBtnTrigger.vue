<script setup>
    import { ref } from 'vue'

    const btnDisable = ref(false)

    function triggerDisabled() {
        btnDisable.value = !btnDisable.value
    }
</script>

<template>
    <div>
        <button :disabled="btnDisable">Button {{ btnDisable }}</button>
        <button @click="triggerDisabled">Trigger</button>
    </div>
</template>