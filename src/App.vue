<template>
  <div id="app">
    <Users />
    <LazyImage data="./404.jpg" />
    <LazyImage data="./test0.jpg" />
    <LazyImage data="./test1.jpg" />
    <LazyImage data="./test2.jpg" />
    <LazyImage data="./test3.jpg" />
    <LazyImage data="./test4.jpg" />
    <LazyImage data="./catdfds.jpg" />
  </div>
</template>

<script>
import Users from "./components/Users.vue"
import LazyImage from "./components/LazyImage.vue"

export default {
  name: 'App',
  components: {
    Users,
    LazyImage
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
