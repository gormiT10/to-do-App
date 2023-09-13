<template>
  <div>
    <div class="task-options-container">
      <div>
        <button v-on:click="changeFormVisibility">Add New Task</button>
        <div>{{ formVisibility }}</div>
      </div>
      <div>
        <button>View My Tasks</button>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
const formVisibility = ref(false);

const changeFormVisibility = () => {
  if (formVisibility === false) {
    return (formVisibility = true);
  } else if (formVisibility === true) {
    return (formVisibility = false);
  }
};
</script>

<style scoped>
.task-options-container {
  margin: 5rem auto;
  width: 30rem;
  display: flex;
  justify-content: space-between;
}
</style>
