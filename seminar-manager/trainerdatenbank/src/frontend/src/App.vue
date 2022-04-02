<template>
  <div id="app">
    <!-- img src="./assets/logo.png"-->
    <NavMenu></NavMenu>
    <router-view/>
  </div>
</template>

<script>
import NavMenu from './components/NavMenu'
export default {
  name: 'App',
  components: {NavMenu},
  mounted() {
    document.title = "Trainerdatenbank";
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
