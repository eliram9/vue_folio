<template>
  <div id="app">
    <FirstScreen />
    <Toolbar />
    <About />
        <br />
    <hr />
        <br />
    <Projects />
    <hr />
        <br />
    <contact /> 
    <hr />
        <br />
    <Footer />         
  </div>
</template>

<script>
import FirstScreen from './components/FirstScreen'
import Toolbar from './components/Toolbar'
import About from './components/About'
import Projects from './components/Projects'
import Contact from './components/Contact'
import Footer from './components/Footer'

export default {
  name: 'app',
  components: {
    FirstScreen,
    Toolbar,
    About,
    Projects,
    Contact,
    Footer
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
