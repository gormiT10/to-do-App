<template>
  <div class="global-container">
    <Profile />
    <TaskOptions />
    <TodosList />
  </div>
</template>

<script setup>
import TaskOptions from "./components/TaskOptions.vue";
import Profile from "./components/Profile.vue";
import TodosList from "./components/TodosList.vue";
</script>

<style scoped>
.global-container {
  width: 60rem;
  margin: 4rem auto;
  background-color: aqua;
}
</style>
