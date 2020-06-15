<template>
  <div id="app">
   
    <dotDash/>
  </div>
</template>

<script>
import dotDash from './components/dotDash.vue';
// import Row from './components/Row.Vue';
export default {
  name: 'App',
  components: {
    dotDash,
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
