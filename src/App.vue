<template>
  <div id="app">
    <!--<img src="./assets/logo.png">-->
    <HelloWorld/>
    <todo-list v-for="(todoItem,index) in items" v-bind:item="todoItem" v-bind:key="index"></todo-list>
  </div>
</template>

<script>
  import HelloWorld from './components/HelloWorld'
  import TodoList from "./components/TodoList";

  export default {
    name: 'App',
    components: {
      TodoList,
      HelloWorld
    },
    data() {
      return {
        items: ['angular', 'vue', 'react']
      }
    }
  }
</script>
A
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
