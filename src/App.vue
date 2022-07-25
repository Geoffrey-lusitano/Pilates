<template>
  <div>
    <App__header/>
    <App__nav/>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'

import App__header from './components/App__header.vue';
import App__nav from './components/App__nav.vue';

export default {
  name: 'App',
  components: {
    App__header,
    App__nav,
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
