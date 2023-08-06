<template>
 <Header />
 <Footer />
 <HomePage />
 <BlogDetails />
 <Blog />

</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import HomePage from './components/HomePage.vue'
import BlogDetails from './components/BlogDetails.vue'
import Blog from './components/Blog.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    HomePage,
    BlogDetails,
    Blog
  }
}
</script>

<style lang="scss">

</style>
