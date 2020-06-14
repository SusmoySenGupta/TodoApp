<template>
  <div id="app" class="container">
    <img alt="Vue logo" src="./assets/logo.png" class="logo" />
    <!-- <TodoList /> -->
    <TodoListEventBus />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import TodoList from "./components/ComponentCommunication/TodoList.vue";
import TodoListEventBus from "./components/EventBus/TodoList.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    TodoList,
    TodoListEventBus
  }
};
</script>

<style>
* {
  box-sizing: border-box;
  text-align: center;
}
.container {
  max-width: 600px;
  margin: 0 auto;
}
.logo {
  height: 75px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  font-size: 24px;
}
</style>
