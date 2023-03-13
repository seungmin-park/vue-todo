<template>
  <section>
    <ul>
      <li v-for="todoItem in todoItems">
        {{ todoItem }}
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  name: "TodoList",
  data() {
    return {
      todoItems: [],
    };
  },

  created() {
    // 로컬 스토리지 데이터 -> 뷰 데이터 저장
    if (localStorage.length > 0) {
      for (let i = 0; i < localStorage.length; i++) {
        this.todoItems.push(localStorage.key(i));
      }
    }
  }
};
</script>

<style scoped>
</style>
