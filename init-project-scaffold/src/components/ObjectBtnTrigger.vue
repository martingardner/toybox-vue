<script>
export default {
    data() {
        return {
            btn: false
        }
    },
    methods: {
        triggerDisabled() {
            this.btn = !this.btn;
        }
    }
}
</script>

<template>
    <span>
    <button :disabled="btn">Button {{btn}}</button>
    <button @click="triggerDisabled">Trigger</button>
    </span>
</template>
