<template>
    <div>
      <input type="checkbox" v-model="task.completed"> 
      <span :class="{ 'completed': task.completed }">{{ task.title }}</span>
      <button @click="editTask">Edit</button>
      <button @click="deleteTask">Delete</button>
    </div>
  </template>
  
  <script>
  export default {
    props: ['task'],
    methods: {
      editTask() {
        // Implementasi edit task
      },
      deleteTask() {
        // Implementasi delete task
      }
    }
  }
  </script>
  
  <style>
  .completed {
    text-decoration: line-through;
  }
  </style>
