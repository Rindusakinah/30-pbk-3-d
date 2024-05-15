<template>
    <div>
      <input type="text" v-model="title" placeholder="Enter task title">
      <button @click="submitForm">{{ editing ? 'Update' : 'Add' }}</button>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        title: '',
        editing: false
      };
    },
    methods: {
      submitForm() {
        if (this.title.trim() === '') return;
        if (this.editing) {
          // Implementasi update task
        } else {
          // Implementasi add task
        }
        this.title = '';
      }
    }
  }
  </script>
  