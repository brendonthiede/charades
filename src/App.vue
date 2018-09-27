<template>
  <div id="app">
    <Charades/>
  </div>
</template>

<script>
import Charades from './components/Charades.vue'

export default {
  name: 'app',
  components: {
    Charades
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
