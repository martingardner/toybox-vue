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
    <div>
    <button :disabled="btn">Button {{btn}}</button>
    <button @click="triggerDisabled">Trigger</button>
    </div>
</template>
