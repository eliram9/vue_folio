<template>
  <div id="app">
    <p>I did it!</p>
    <FirstScreen />
  </div>
</template>

<script>
import FirstScreen from './components/FirstScreen'

export default {
  name: 'app',
  components: {
    FirstScreen
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
