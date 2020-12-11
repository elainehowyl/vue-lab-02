<template>
  <div id="app">
    <ControlPanel></ControlPanel>
    <MainCounter></MainCounter>
  </div>
</template>

<script>
import ControlPanel from "./components/ControlPanel"
import MainCounter from "./components/MainCounter"

export default {
  name: 'App',
  components: {
    ControlPanel, MainCounter
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
