<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld v-bind:msg="title"/>
    <HelloWorld v-bind:msg="getTitle()"/>
    <!-- short v-bind -->
    <HelloWorld :msg="title"/> 
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  data() {
    return {
      title: "Some Title",
    }
  },
  components: {
    HelloWorld
  },
  methods: {
    getTitle() {
      return this.title + "!!!";
    }
  },
}
</script>
