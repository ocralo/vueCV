<template>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
</template>

<script>
import HelloWorld from './views/index.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
  }
}
</script>

<style>
html,body {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  background-color: #1D1A26;
  color: #ffffff;
  height: 100vh;
  margin: 0;
}
</style>
