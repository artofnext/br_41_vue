<template>
  <div>
   <h1 v-once>{{ title }}</h1>
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

      this.title = "Other title";
      return this.title;
    }
  }
}
</script>