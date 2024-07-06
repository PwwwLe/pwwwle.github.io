<!-- Home.vue -->
<template>
  <div>
    <h1>Home</h1>
    <p>Welcome to my blog!</p>
  </div>
</template>

<script>
import blogList from "../components/BlogList.vue";

export default {
  name: 'Home',
  components: {
    blogList,
  },
};
</script>

<style scoped>
h1 {
  color: #42b983;
}
</style>