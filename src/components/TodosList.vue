<template>
  <div class="to-dos-block">
    <table>
      <tbody>
        <td>Title</td>
        <td>Description</td>
        <td>Due Date</td>
        <td>Categorie</td>
        <td>Priority</td>
        <td>Status</td>
        <tr v-for="todo in state.savedToDos" :key="todo.title">
          <td>{{ todo.title }}</td>
          <td>{{ todo.description }}</td>
          <td>{{ todo.dueDate }}</td>
          <td>{{ todo.categorie }}</td>
          <td>{{ todo.priority }}</td>
          <td>{{ todo.status }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script setup>
import { reactive, onMounted } from "vue";
const state = reactive({
  savedToDos: [],
});

onMounted(() => {
  state.savedToDos = [
    {
      title: "code",
      description: "time-to-code",
      dueDate: "tomorrow",
      categorie: "career",
      priority: "high",
      status: "Undone",
    },
    {
      title: "read my bible",
      description: "time-to-code",
      dueDate: "tomorrow",
      categorie: "career",
      priority: "high",
      status: "Undone",
    },

    {
      title: "feed animals",
      description: "time-to-code",
      dueDate: "tomorrow",
      categorie: "career",
      priority: "high",
      status: "Undone",
    },
  ];
});
</script>

<style scoped>
.to-dos-block {
  padding-bottom: 10rem;
}

/* styles.css */
table {
  width: 100%;
  border-collapse: collapse;
}

th,
td {
  border: 1px solid #ddd;
  padding: 8px;
  text-align: left;
}

th {
  background-color: #f2f2f2;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
}

/* Add more styles as needed */
</style>
