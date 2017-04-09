<template>
  <div id="app">
    <img src="./assets/logo.png">
    <shelfy></shelfy>
  </div>
</template>

<script>
import Shelfy from './components/shelfy'

export default {
  name: 'app',
  components: {
    Shelfy
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
