<template>
    <div>
        <h1>{{ counter }}</h1>
        <br>
        <button v-on:click="increaseCounter">Increase</button>
        <button @click="decreaseCounter">Decrease</button>
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
            console.log('Click increase');
        },
        decreaseCounter() {
            this.counter--;
            console.log('Click decrease');
        },

    }
}
</script>