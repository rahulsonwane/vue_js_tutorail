<template>
  <!-- <HelloWorld msg="Welcome to AWS Project" /> -->
  <!-- <HomeWorld/> -->
  <!-- <TwoWayBind/> -->
  <!-- <GetInputField/> -->
  <!-- <CheckRadiBut/> -->
  <!-- <IfElse/> -->
  <!-- <ForLoop/> -->
  <!-- <BaseHome/> -->
  <!-- <ReuseCompo/> -->
  <!-- <HtmlBin/> -->
  <!-- <ClassBin/> -->
  <!-- <PropBase/> -->
  <!-- <RefDom/> -->
  <!-- <MakeForm/> -->
  <!-- <FormModifier/> -->
  <!-- <PassNonProps/> -->
  <!-- <WaTchers/> -->
<!-- <BaseSlot/> -->
<!-- <DnyCom/> -->
<Teleport to="#footer">
  <FooterTele/>
</Teleport>

</template>


<script>
import FooterTele from './components/FooterTele.vue';
// import FormModifier from './components/FormModifier.vue';
// import PassNonProps from './components/PassNonProps.vue';

// import BaseSlot from './components/BaseSlot.vue';
// import DnyCom from './components/DnyCom.vue';
// import WaTchers from './components/WaTchers.vue';


// import BaseHome from './components/BaseHome.vue';
// import ClassBin from './components/ClassBin.vue';
// import PropBase from './components/PropBase.vue';
// import MakeForm from './components/MakeForm.vue';
// import RefDom from './components/RefDom.vue';
// import HtmlBin from './components/HtmlBin.vue';
// import ReuseCompo from './components/ReuseCompo.vue';
// import HelloWorld from './components/HelloWorld.vue';
// import HomeWorld from './components/HomeWorld.vue';
// import TwoWayBind from './components/TwoWayBind.vue';
// import GetInputField from './components/GetInputField.vue';
// import CheckRadiBut from './components/CheckRadiBut.vue';
// import ForLoop from './components/ForLoop.vue';
// import IfElse from './components/IfElse.vue';



export default {
  name: 'App',
  components: {
    // FormModifier,
    // PassNonProps,
    // WaTchers,
    // BaseSlot,
    // DnyCom,
    FooterTele
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
