<template>
    <div>
      <button @click="fetchData">Fetch Comments</button>
      <pre v-if="comments">{{ comments }}</pre>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        comments: null,
      };
    },
    methods: {
      async fetchData() {
        try {
          const response = await fetch('https://jsonplaceholder.typicode.com/comments');
          this.comments = await response.json();
        } catch (error) {
          console.error('Error fetching comments:', error);
        }
      }
    }
  };
  </script>
  
  <style scoped>
  /* Add any specific styling for your card component */
  </style>
  