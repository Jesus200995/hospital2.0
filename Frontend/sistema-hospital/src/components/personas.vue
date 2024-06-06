<template>
    <div class="form-container">
      <h1>Registro de Personas</h1>
      <form @submit.prevent="submitForm">
        <div class="form-group">
          <label for="nombre">Nombre:</label>
          <input type="text" id="nombre" v-model="form.nombre" required />
        </div>
        <div class="form-group">
          <label for="apellidoPaterno">Apellido Paterno:</label>
          <input type="text" id="apellidoPaterno" v-model="form.apellidoPaterno" required />
        </div>
        <div class="form-group">
          <label for="apellidoMaterno">Apellido Materno:</label>
          <input type="text" id="apellidoMaterno" v-model="form.apellidoMaterno" required />
        </div>
        <div class="form-group">
          <label for="curp">CURP:</label>
          <input type="text" id="curp" v-model="form.curp" required />
        </div>
        <div class="form-group">
          <label for="genero">Género:</label>
          <select id="genero" v-model="form.genero" required>
            <option value="" disabled>Seleccione</option>
            <option value="masculino">Masculino</option>
            <option value="femenino">Femenino</option>
            <option value="otro">Otro</option>
          </select>
        </div>
        <div class="form-group">
          <label for="tipoSangre">Tipo de Sangre:</label>
          <select id="tipoSangre" v-model="form.tipoSangre" required>
            <option value="" disabled>Seleccione</option>
            <option value="A+">A+</option>
            <option value="A-">A-</option>
            <option value="B+">B+</option>
            <option value="B-">B-</option>
            <option value="AB+">AB+</option>
            <option value="AB-">AB-</option>
            <option value="O+">O+</option>
            <option value="O-">O-</option>
          </select>
        </div>
        <div class="form-group">
          <label for="fechaNacimiento">Fecha de Nacimiento:</label>
          <input type="date" id="fechaNacimiento" v-model="form.fechaNacimiento" required />
        </div>
        <div class="form-group">
          <label for="telefono">Teléfono:</label>
          <input type="tel" id="telefono" v-model="form.telefono" required />
        </div>
        <div class="form-group">
          <label for="correo">Correo Electrónico:</label>
          <input type="email" id="correo" v-model="form.correo" required />
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
          nombre: '',
          apellidoPaterno: '',
          apellidoMaterno: '',
          curp: '',
          genero: '',
          tipoSangre: '',
          fechaNacimiento: '',
          telefono: '',
          correo: ''
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
  
  .form-group input,
  .form-group select {
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
  