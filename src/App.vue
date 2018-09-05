<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Home :msg="message"/>
    <counter></counter>
  </div>
</template>

<script>
import Vue from 'vue';
import Home from './components/Home.vue';
import Counter from './components/Counter.vue';

export default Vue.component('App', {
  name: 'app',
  data() {
    return {
      message: 'VueJs Counter',
    };
  },
  components: {
    Home,
    Counter,
  },
});
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
