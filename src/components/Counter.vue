<template>
    <div>
        <h1>{{ counter }}</h1>
        <br>
        <button v-on:click="increaseCounter">Increase</button>
        <button @click="decreaseCounter">Decrease</button>
        <form>
            <input type="submit"  @click.prevent="decreaseCounter" value="Decrease NoSubmit">
        </form>
    </div>
</template>

<script>

// v-[directive]:[attribute].[modifier]

export default {
    name: "Counter",
    data() {
        return {
            counter: 0,
        }
    },
    methods: {
        increaseCounter(event) {


            console.log(event);
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