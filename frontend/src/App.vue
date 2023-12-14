<template>
  <div>
    <form @submit.prevent="submitForm">
      <label for="nama">Nama:</label>
      <input type="text" id="nama" v-model="formData.nama" required>

      <label for="email">Email:</label>
      <input type="email" id="email" v-model="formData.email" required>

      <label for="asalSekolah">Asal Sekolah:</label>
      <input type="text" id="asalSekolah" v-model="formData.asalSekolah" required>

      <button type="submit">Daftar</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      formData: {
        nama: '',
        email: '',
        asalSekolah: '',
      },
    };
  },
  methods: {
    submitForm() {
      
      console.log('Data Pendaftaran:', this.formData);
      
      this.formData = {
        nama: '',
        email: '',
        asalSekolah: '',
      };
    },
  },
};
</script>

<style scoped>
form {
  max-width: 400px;
  margin: 0 auto;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 5px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

label {
  display: block;
  margin-bottom: 8px;
  font-weight: bold;
}

input {
  width: 100%;
  padding: 8px;
  margin-bottom: 16px;
  box-sizing: border-box;
  border: 1px solid #ccc;
  border-radius: 4px;
}

button {
  background-color: #4caf50;
  color: white;
  padding: 10px 15px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
}

button:hover {
  background-color: #45a049;
}
</style>
