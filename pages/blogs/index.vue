<template>
  <section>
    <h1>Blogs Page</h1>
    <ul>
      <li v-for="blog of 5" :key="blog">
       <a href="#" @click.prevent="openBlog(blog)">Blog {{blog}}</a>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  methods: {
    openBlog(blog) {
      this.$router.push('/blogs/' + blog.id)
    }
  }
}
</script>