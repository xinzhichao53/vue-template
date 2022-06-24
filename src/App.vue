<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/>
  <test-demo1></test-demo1>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import TestDemo1 from './components/TestDemo1.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    TestDemo1,
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
  margin-top: 60px;
}
</style>
