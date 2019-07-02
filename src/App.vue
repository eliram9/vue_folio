<template>
  <div id="app">
    <FirstScreen />
    <hr />
        <br />
    <About />
        <br />
    <hr />
        <br />
    <Projects />    
  </div>
</template>

<script>
import FirstScreen from './components/FirstScreen'
import About from './components/About'
import Projects from './components/Projects'

export default {
  name: 'app',
  components: {
    FirstScreen,
    About,
    Projects
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
}
</style>
