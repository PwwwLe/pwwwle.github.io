<template>
  <div>
    <h2>{{ post.title }}</h2>
    <p>{{ post.content }}</p>
  </div>
</template>

<script>
export default {
  name: 'Post',
  data() {
    return {
      post: {
        title: 'Blog Post Title',
        content: 'Blog post content...',
      },
    };
  },
  created() {
    const postId = this.$route.params.id;
    // Fetch the post data based on postId
    // For now, we're using static data
    if (postId === '1') {
      this.post = {title: 'First Blog Post', content: 'Content of the first blog post.'};
    } else if (postId === '2') {
      this.post = {title: 'Second Blog Post', content: 'Content of the second blog post.'};
    }
  },
};
</script>

<style scoped>
h2 {
  color: #42b983;
}
</style>