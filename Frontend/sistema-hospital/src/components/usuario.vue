<template>
    <div class="form-container">
      <h1>Registro de Usuario</h1>
      <form @submit.prevent="submitForm">
        <div class="form-group">
          <label for="usuario">Usuario:</label>
          <input type="text" id="usuario" v-model="form.usuario" required />
        </div>
        <div class="form-group">
          <label for="contrasena">Contraseña:</label>
          <input type="password" id="contrasena" v-model="form.contrasena" required />
        </div>
        <button type="submit">Registrar</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        form: {
          usuario: '',
          contrasena: ''
        }
      };
    },
    methods: {
      submitForm() {
        // Aquí puedes manejar el envío del formulario, por ejemplo, enviando los datos a una API
        console.log(this.form);
      }
    }
  };
  </script>
  
  <style scoped>
  .form-container {
    max-width: 600px;
    margin: 0 auto;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    background-color: #f9f9f9;
  }
  
  h1 {
    text-align: center;
    margin-bottom: 20px;
  }
  
  .form-group {
    margin-bottom: 15px;
  }
  
  .form-group label {
    display: block;
    margin-bottom: 5px;
    font-weight: bold;
  }
  
  .form-group input {
    width: 100%;
    padding: 8px;
    box-sizing: border-box;
    border: 1px solid #ccc;
    border-radius: 5px;
  }
  
  button {
    display: block;
    width: 100%;
    padding: 10px;
    background-color: #007bff;
    color: white;
    border: none;
    border-radius: 5px;
    font-size: 16px;
    cursor: pointer;
  }
  
  button:hover {
    background-color: #0056b3;
  }
  </style>
  