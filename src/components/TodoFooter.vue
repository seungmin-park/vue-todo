<template>
<div class="clearAllContainer">
  <span class="clearBtn" @click="clearTodo">Clear All</span>
</div>
</template>

<script>
export default {
  name: "TodoFooter",
  methods: {
    clearTodo() {
      localStorage.clear();
    },
  },
}
</script>

<style scoped>

</style>
