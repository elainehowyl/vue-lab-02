<template>
  <div id="app" class="container">
    <TodoList></TodoList>
    <ProductList></ProductList>
    <TodoListAdvanced></TodoListAdvanced>
  </div>
</template>

<script>
import TodoList from "./components/TodoList"
import ProductList from "./components/ProductList"
import TodoListAdvanced from "./components/TodoListAdvanced"

export default {
  name: 'App',
  components: {
    TodoList, ProductList, TodoListAdvanced
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
