<template>
  <div id="app">
    <img src="./assets/logo.png">
    <br>
<!--    <hello></hello> -->
<div style="margin:auto;width: 610px">
    <component1></component1>
    <component2></component2>
</div>
  </div>
</template>

<script>

import Component1 from './components/Component1';
import Component2 from './components/Component2';

export default {
  name: 'app',
  components: {
    Component1, Component2
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
