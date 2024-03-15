<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <PAGES />
  <inputBoxes />
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue';
import PAGES from './components/New-one.vue';
import inputBoxes from './components/Input-boxes.vue';

export default {
  name: 'App',
  components: {
    // HelloWorld,
    PAGES,
    inputBoxes,

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
