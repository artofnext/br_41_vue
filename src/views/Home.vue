<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld v-bind:msg="title"/>
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
  }
}
</script>
