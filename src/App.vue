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
@import url('https://fonts.googleapis.com/css2?family=M+PLUS+Rounded+1c:wght@300;400;500&display=swap');
:root {
  --color-primary: #9F366E;
  --color-secondady: #C98FAE;
  --color-text-menu: #FFFAFA;
}
#app {
  font-family: "M PLUS Rounded 1c", Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 60px;
}
</style>
