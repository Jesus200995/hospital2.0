<template>
  <div class="min-h-screen bg-gray-50 flex flex-col justify-center py-12 sm:px-6 lg:px-8">
    <div class="sm:mx-auto sm:w-full sm:max-w-md">
      <img class="mx-auto h-10 w-auto" src="https://www.svgrepo.com/show/301692/login.svg" alt="Workflow">
      <h2 class="mt-6 text-center text-3xl leading-9 font-extrabold text-gray-900">
        Crea una cuenta nueva
      </h2>
      <p class="mt-2 text-center text-sm leading-5 text-gray-500 max-w">
        O
        <router-link to="/login" class="font-medium text-blue-600 hover:text-blue-500 focus:outline-none focus:underline transition ease-in-out duration-150">
          Inicia sesión en tu cuenta
        </router-link>
      </p>
    </div>

    <div class="mt-8 sm:mx-auto sm:w-full sm:max-w-md">
      <div class="bg-white py-8 px-4 shadow sm:rounded-lg sm:px-10">
        <form method="POST" action="#">
          <div class="space-y-6">
            <div>
              <label for="name" class="block text-sm font-medium leading-5 text-gray-700">Nombre</label>
              <div class="mt-1">
                <input id="name" name="name" placeholder="Ingrese su nombre" type="text" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md placeholder-gray-400 focus:outline-none focus:shadow-outline-blue focus:border-blue-300 transition duration-150 ease-in-out sm:text-sm sm:leading-5">
              </div>
            </div>

            <div>
              <label for="primerApellido" class="block text-sm font-medium leading-5 text-gray-700">Primer Apellido</label>
              <div class="mt-1">
                <input id="primerApellido" name="primerApellido" placeholder="Ingrese su primer apellido" type="text" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md placeholder-gray-400 focus:outline-none focus:shadow-outline-blue focus:border-blue-300 transition duration-150 ease-in-out sm:text-sm sm:leading-5">
              </div>
            </div>

            <div>
              <label for="segundoApellido" class="block text-sm font-medium leading-5 text-gray-700">Segundo Apellido</label>
              <div class="mt-1">
                <input id="segundoApellido" name="segundoApellido" placeholder="Ingrese su segundo apellido" type="text" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md placeholder-gray-400 focus:outline-none focus:shadow-outline-blue focus:border-blue-300 transition duration-150 ease-in-out sm:text-sm sm:leading-5">
              </div>
            </div>

            <div>
              <label for="curp" class="block text-sm font-medium leading-5 text-gray-700">CURP</label>
              <div class="mt-1">
                <input id="curp" name="curp" placeholder="Ingrese su CURP" type="text" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md placeholder-gray-400 focus:outline-none focus:shadow-outline-blue focus:border-blue-300 transition duration-150 ease-in-out sm:text-sm sm:leading-5">
              </div>
            </div>

            <div>
              <label for="genero" class="block text-sm font-medium leading-5 text-gray-700">Género</label>
              <div class="mt-1">
                <select id="genero" name="genero" required class="block w-full px-3 py-2 border border-gray-300 bg-white rounded-md shadow-sm focus:outline-none focus:shadow-outline-blue focus:border-blue-300 transition duration-150 ease-in-out sm:text-sm sm:leading-5">
                  <option value="">Seleccione su género</option>
                  <option value="masculino">Masculino</option>
                  <option value="femenino">Femenino</option>
                  <option value="nobinario">No Binario</option>
                  <option value="otro">Otro</option>
                </select>
              </div>
            </div>

            <div>
              <label for="sangre" class="block text-sm font-medium leading-5 text-gray-700">Tipo de Sangre</label>
              <div class="mt-1">
                <input id="sangre" name="sangre" placeholder="Ingrese su tipo de sangre" type="text" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md placeholder-gray-400 focus:outline-none focus:shadow-outline-blue focus:border-blue-300 transition duration-150 ease-in-out sm:text-sm sm:leading-5">
              </div>
            </div>

            <div>
              <label for="fechaNacimiento" class="block text-sm font-medium leading-5 text-gray-700">Fecha de Nacimiento</label>
              <div class="mt-1">
                <input id="fechaNacimiento" name="fechaNacimiento" type="date"
 required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md placeholder-gray-400 focus:outline-none focus:shadow-outline-blue focus:border-blue-300 transition duration-150 ease-in-out sm:text-sm sm:leading-5">
              </div>
            </div>

            <div>
              <label for="telefono" class="block text-sm font-medium leading-5 text-gray-700">Teléfono</label>
              <div class="mt-1">
                <input id="telefono" name="telefono" placeholder="Ingrese su teléfono" type="text" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md placeholder-gray-400 focus:outline-none focus:shadow-outline-blue focus:border-blue-300 transition duration-150 ease-in-out sm:text-sm sm:leading-5">
              </div>
            </div>

            <div>
              <label for="email" class="block text-sm font-medium leading-5 text-gray-700">Correo Electrónico</label>
              <div class="mt-1">
                <input id="email" name="email" placeholder="user@example.com" type="email" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md placeholder-gray-400 focus:outline-none focus:shadow-outline-blue focus:border-blue-300 transition duration-150 ease-in-out sm:text-sm sm:leading-5">
              </div>
            </div>

            <div>
              <label for="username" class="block text-sm font-medium leading-5 text-gray-700">Nombre de Usuario</label>
              <div class="mt-1">
                <input id="username" name="username" placeholder="Ingrese su nombre de usuario" type="text" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md placeholder-gray-400 focus:outline-none focus:shadow-outline-blue focus:border-blue-300 transition duration-150 ease-in-out sm:text-sm sm:leading-5">
              </div>
            </div>

            <div>
              <label for="password" class="block text-sm font-medium leading-5 text-gray-700">Contraseña</label>
              <div class="mt-1">
                <input id="password" name="password" type="password" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md placeholder-gray-400 focus:outline-none focus:shadow-outline-blue focus:border-blue-300 transition duration-150 ease-in-out sm:text-sm sm:leading-5">
              </div>
            </div>

            <div>
              <label for="password_confirmation" class="block text-sm font-medium leading-5 text-gray-700">Repetir Contraseña</label>
              <div class="mt-1">
                <input id="password_confirmation" name="password_confirmation" type="password" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md placeholder-gray-400 focus:outline-none focus:shadow-outline-blue focus:border-blue-300 transition duration-150 ease-in-out sm:text-sm sm:leading-5">
              </div>
            </div>

          </div>

          <div class="mt-6">
            <span class="block w-full rounded-md shadow-sm">
              <button type="submit" class="w-full flex justify-center py-2 px-4 border border-transparent text-sm font-medium rounded-md text-white bg-blue-600 hover:bg-blue-500 focus:outline-none focus:border-indigo-700 focus:shadow-outline-indigo active:bg-indigo-700 transition duration-150 ease-in-out">
                Create account
              </button>
            </span>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'RegisterForm',
}
</script>

<style scoped>
/* Agrega cualquier estilo adicional que necesites aquí */
</style>