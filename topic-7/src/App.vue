<template>
  <div id="app" class="container">
    <TodoList></TodoList>
    <ProductList></ProductList>
  </div>
</template>

<script>
import TodoList from "./components/TodoList"
import ProductList from "./components/ProductList"


export default {
  name: 'App',
  components: {
    TodoList, ProductList
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
