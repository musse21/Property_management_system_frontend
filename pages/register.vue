<template>
    <div>
      <h2 class="text-2x1 font-bold mb-6 text-center">Property Management System</h2>
      <h3 class="text-2xl font-bold mb-6 text-center drop-shadow-lg">Register</h3>
      <form @submit.prevent="register">
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="firstName">First Name</label>
          <input type="text" v-model="firstName" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" required>
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="lastName">Last Name</label>
          <input type="text" v-model="lastName" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" required>
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="email">Email</label>
          <input type="email" v-model="email" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" required>
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="phone">Phone</label>
          <input type="tel" v-model="phone" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" required>
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="age">Age</label>
          <input type="number" v-model="age" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" required>
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="sex">Sex</label>
          <select v-model="sex" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline">
            <option value="male">Male</option>
            <option value="female">Female</option>
          </select>
        </div>
        <div class="mb-6">
          <label class="block text-gray-700 text-sm font-bold mb-2" for="password">Password</label>
          <input type="password" v-model="password" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" required>
        </div>
        <div class="flex items-center justify-center">
          <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline" type="submit">Register</button>
        </div>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    layout: 'auth',
    data() {
      return {
        firstName:'',
        lastName:'',
        email: '',
        phone: '',
        age: '',
        sex: '',
        password: ''
      }
    },
    methods: {
      register() {
        // Handle register logic
        console.log('First Name:', this.firstName, 'Last Name:', this.lastName ,'Email:', this.email, 'Phone:', this.phone, 'Age:', this.age, 'Sex:', this.sex, 'Password:', this.password);
      }
    }
  }
  </script>
  