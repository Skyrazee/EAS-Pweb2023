<template>
    <div>
      <h2>Cek Status Pendaftaran</h2>
      <form @submit.prevent="checkStatus">
        <label for="checkEmail">Email:</label>
        <input type="email" id="checkEmail" v-model="email" required>
        <button type="submit">Cek Status</button>
      </form>
  
      <div v-if="status !== null">
        <h3>Status Pendaftaran:</h3>
        <p>{{ status }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        email: '',
        status: null,
      };
    },
    methods: {
      checkStatus() {
        // Simulate server request to check registration status
        // In a real application, you would make an API call here
        // For simplicity, let's assume the status is fetched from a server
        // Update the status based on the actual logic
        this.status = Math.random() > 0.5 ? 'Terverifikasi' : 'Belum Terverifikasi';
      },
    },
  };
  </script>
  
  <style scoped>
  /* Add your styling for the CheckStatus component */
  </style>
  