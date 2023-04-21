<template>
  <HelloWorld msg="Welcome to AWS Project" />
  <!-- <HomeWorld/> -->
  <!-- <TwoWayBind/> -->
  <!-- <GetInputField/> -->
  <!-- <CheckRadiBut/> -->
  <!-- <IfElse/> -->
  <!-- <ForLoop/> -->
</template>


<script>

import HelloWorld from './components/HelloWorld.vue';
// import HomeWorld from './components/HomeWorld.vue';
// import TwoWayBind from './components/TwoWayBind.vue';
// import GetInputField from './components/GetInputField.vue';
// import CheckRadiBut from './components/CheckRadiBut.vue';
// import ForLoop from './components/ForLoop.vue';
// import IfElse from './components/IfElse.vue';


export default {
  name: 'App',
  components: {
    // HomeWorld,
    HelloWorld,
    // TwoWayBind,
    // GetInputField,
    // CheckRadiBut,
    // IfElse,
    // ForLoop
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
