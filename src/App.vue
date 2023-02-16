<template>

  <NavBar/>

  <div class="mt-4 mb-4">
    <router-view :blogWrite="blogWrite"></router-view>
  </div>


</template>

<script>
import blog from './assets/data'
import NavBar from './components/NavBar.vue'

export default {
  name: 'App',
  data() {
    return {
      blogWrite : blog
    }
  },
  components: {
    NavBar
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
