<template>
  <div>
   <h1 v-once>{{ title }}</h1>
   <p>{{ getTitle() }}</p>
   <a v-bind:href="url">Google</a>
  </div>
</template>

<script>
export default {
  name: 'app',
  data() {
    return {
      title: "Some Title",
      url: "https://google.com",
    }
  },
  methods: {
    getTitle() {

      this.title = "Other title";
      return this.title;
    }
  }
}
</script>