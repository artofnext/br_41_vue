<template>
  <div id="app">
   <h1>{{ title }}</h1>
   <p>{{ getTitle() }}</p>
  </div>
</template>

<script>
export default {
  name: 'app',
  data() {
    return {
      title: "Some Title",
      url: "",
    }
  },
  methods: {
    getTitle() {
      return this.title;
    }
  }
}
</script>