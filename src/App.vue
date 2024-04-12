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
  <slotComp>
    <template v-slot:header>
      <div>
        <h3>GOLO Betsalel this is the header</h3>
      </div>
    </template>

    <template v-slot:main>
      <div>
        <h3>GOLO Betsalel this is the main</h3>
      </div>
    </template>

    <template v-slot:footer>
      <div>
        <h3>GOLO Betsalel this is the footer</h3>
      </div>
    </template>
  </slotComp>
  <slotComp>
    <template v-slot:header>
      <div>
        <h3>GOLO Betsalel this is the fake header</h3>
      </div>
    </template>

    <template v-slot:main>
      <div>
        <h3>GOLO Betsalel this is the fake main</h3>
      </div>
    </template>

    <template v-slot:footer>
      <div>
        <h3>GOLO Betsalel this is the fake footer</h3>
      </div>
    </template>
  </slotComp>
  <home/>
  
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
import slotComp from './components/slots.vue';
import homeComp from './components/home.vue';

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
    watcherComp,
    slotComp,
    homeComp

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
