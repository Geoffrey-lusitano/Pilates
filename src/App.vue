<template>
  <div>
    <App__header/>
    <App__nav/>
    <App__about/>
    <App__pilates/>
    <App__ht/>
    <App__contact/>
    <App__footer/>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'

import App__header from './components/App__header.vue';
import App__nav from './components/App__nav.vue';
import App__about from './components/App__about.vue';
import App__pilates from './components/App__pilates.vue';
import App__ht from './components/App__ht.vue';
import App__contact from './components/App__contact.vue';
import App__footer from './components/App__footer.vue';


export default {
  name: 'App',
  components: {
    App__header,
    App__nav,
    App__about,
    App__pilates,
    App__ht,
    App__contact,
    App__footer
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
