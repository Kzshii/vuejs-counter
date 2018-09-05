<template>
<section class="section">
  <div class="container">
    <div class="level">
      <div class="level-item">
        <button style="padding: 5px 20px" class="button" @click="incrementCounter">Increment</button>
      </div>
      <div class="level-item">
        <h2>{{counter}}</h2>
      </div>
      <div class="level-item">
        <button class="button" style="padding: 5px 20px" @click="decrementCounter">Decrement</button>
      </div>
    </div>
  </div>
</section>
</template>

<script>
import Vue from 'vue';

export default Vue.component('Counter', {
  data() {
    return {
      title: 'Counter',
      counter: 0,
    };
  },
  methods: {
    incrementCounter() {
      this.counter++;
    },
    decrementCounter() {
      this.counter--;
    },
  },
});
</script>
