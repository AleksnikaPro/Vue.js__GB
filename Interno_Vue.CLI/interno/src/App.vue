<template>
  <Header />
  <Footer />
  <HomePage />
  <BlogDetails />
  <Blog />
  <Project />
  <ProjectDetails/>
  <NotFound />
  <!-- <Slider /> -->
 
 </template>
 
 <script>
 import Header from './components/Header.vue'
 import Footer from './components/Footer.vue'
 import HomePage from './components/HomePage.vue'
 import BlogDetails from './components/BlogDetails.vue'
 import Blog from './components/Blog.vue'
 import Project from './components/Project.vue'
 import ProjectDetails from './components/ProjectDetails.vue'
 import NotFound from './components/NotFound.vue'
 import Slider from './components/Slider.vue'
 
 export default {
   name: 'App',
   components: {
     Header,
     Footer,
     HomePage,
     BlogDetails,
     Blog,
     Project,
     ProjectDetails,
     NotFound,
     Slider
   }
 }
 </script>
 <style lang="scss"></style>
 


<!-- <template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav>
  <router-view/>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style> -->
