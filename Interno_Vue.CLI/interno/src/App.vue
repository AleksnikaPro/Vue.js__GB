<template>
 <Header />
 <Footer />
 <HomePage />
 <BlogDetails />
 <Blog />
 <Project />

</template>

<script>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import HomePage from './components/HomePage.vue'
import BlogDetails from './components/BlogDetails.vue'
import Blog from './components/Blog.vue'
import Project from './components/Project.vue'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
    HomePage,
    BlogDetails,
    Blog,
    Project
  }
}
</script>
<style lang="scss"></style>
