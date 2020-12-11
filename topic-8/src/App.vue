<template>
  <div id="app">
    <TodoListAdvanced></TodoListAdvanced>
    <ProductListAdvanced></ProductListAdvanced>
  </div>
</template>

<script>
import TodoListAdvanced from "./components/TodoListAdvanced"
import ProductListAdvanced from "./components/ProductListAdvanced"
export default {
  name: 'App',
  components: {
    TodoListAdvanced, ProductListAdvanced
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
