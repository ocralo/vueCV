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
body {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  background-color: #1D1A26;
  background-image: url("~@/assets/img/fondo_cv.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  color: #ffffff;
  margin: 0;
}
</style>
