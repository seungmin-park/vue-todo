<template>
  <div id="app">
    <TodoHeader></TodoHeader>
  </div>
</template>

<script>
import TodoHeader from "./components/TodoHeader.vue";

export default {
  components: {
    "TodoHeader": TodoHeader,
  }
}
</script>

<style>
body {
  text-align: center;
  background-color: #F6F6F8;
}
</style>
