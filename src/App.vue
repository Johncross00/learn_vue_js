<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <!-- <PAGES /> -->
  <inputBoxes />
  <!-- <conditionComp /> -->
  <!-- <forLoop /> -->
  <!-- <mainComp /> -->
  <formComp />
  <props/>
  <computyProp />
  <watcherComp />
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue';
// import PAGES from './components/New-one.vue';
// import inputBoxes from './components/Input-boxes.vue';
// import conditionComp from './components/conditions.vue';
// import forLoop from './components/forLoop.vue';
// import mainComp from './components/school.vue';
import formComp from './components/form.vue';
import props from './components/props.vue';
import computyProp from './components/computyProp.vue';
import watcherComp from './components/watcher.vue';

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // PAGES,
    // inputBoxes,
    // conditionComp,
    // forLoop,
    // mainComp,
    formComp,
    props,
    computyProp,
    watcherComp

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
