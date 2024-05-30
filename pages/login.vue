<template>
  <div>
    <h2 class="text-2x1 font-bold mb-6 text-center">Property Management System</h2>
    <h2 class="text-2xl font-bold mb-6 text-center">Login</h2>
    <form @submit.prevent="login">
      <div class="mb-4">
        <label class="block text-gray-700 text-sm font-bold mb-2" for="email">Email</label>
        <input type="email" v-model="email" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" required>
      </div>
      <div class="mb-6">
        <label class="block text-gray-700 text-sm font-bold mb-2" for="password">Password</label>
        <input type="password" v-model="password" class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline" required>
      </div>
      <div class="flex items-center justify-center">
        <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline" type="submit">Login</button>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  layout: 'auth',
  data() {
    return {
      email: '',
      password: ''
    }
  },
  methods: {
    login() {
      // Handle login logic
      console.log('Email:', this.email, 'Password:', this.password);
    }
  }
}
</script>
