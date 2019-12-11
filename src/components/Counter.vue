<template>
    <div>
        <h1>{{ counter }}</h1>
        <br>
        <button v-on:click="increaseCounter">Increase</button>
    </div>
</template>

<script>
export default {
    name: "Counter",
    data() {
        return {
            counter: 0,
        }
    },
    methods: {
        increaseCounter() {
            this.counter++;
        }
    }
}
</script>