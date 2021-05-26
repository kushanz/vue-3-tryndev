<template>
  <div id="app">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <h3>{{ counter }}</h3>
    <button @click="increment">Count</button>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import { ref } from 'vue'
export default {
  name: 'App',
  components: {
    HelloWorld
  },
  setup() {
    const counter = ref(0)
    const increment = () => {counter.value++}

    return {counter,increment}
    
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
