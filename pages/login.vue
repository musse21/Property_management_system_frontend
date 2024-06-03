<template>
  <div
    class="min-h-screen flex items-center justify-center bg-cover bg-center bg-no-repeat bg-auth-layout"
  >
    <div
      class="max-w-md w-full bg-zinc-200 bg-opacity-75 shadow-md rounded-lg p-8"
    >
      <div class="mb-8">
        <h2 class="text-2xl font-bold text-black mb-6 text-center">
          Property Management System
        </h2>
        <h2 class="text-2xl font-bold text-black mb-6 text-center">Login</h2>
        <form @submit.prevent="login">
          <div class="mb-4">
            <label class="block text-black text-sm font-bold mb-2" for="email"
              >Email</label
            >
            <input
              type="email"
              v-model="email"
              class="shadow appearance-none border rounded w-full py-2 px-3 text-black leading-tight focus:outline-none focus:shadow-outline"
              required
            />
          </div>
          <div class="mb-6">
            <label
              class="block text-black text-sm font-bold mb-2"
              for="password"
              >Password</label
            >
            <input
              type="password"
              v-model="password"
              class="shadow appearance-none border rounded w-full py-2 px-3 text-black leading-tight focus:outline-none focus:shadow-outline"
              required
            />
          </div>
          <div class="flex items-center justify-center">
            <button
              class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline"
              type="submit"
            >
              Login
            </button>
          </div>
          <div class="flex items-center justify-center pt-3">
            <button
              @click="loginWith('google')"
              class="bg-green-500 hover:bg-green-600 text-white font-bold py-2 px-4 rounded mb-4"
            >
            <i class="fa-brands fa-google text-sm pl-2" style="text-transform: none;"> Signin with Google</i>
            </button>
          </div>
        </form>
      </div>

      <div class="mt-4">
        <h2 class="text-2xl font-bold text-black mb-6 text-center">Or</h2>
        <router-link
          to="/register"
          class="w-full bg-blue-500 hover:bg-blue-600 text-white font-bold py-2 px-4 rounded mb-4 block text-center"
        >
          Signup
        </router-link>
        <router-link
          to="/"
          class="w-full bg-red-500 hover:bg-red-600 text-white font-bold py-2 px-4 rounded mb-4 block text-center"
        >
          Back Home
        </router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AuthLayout",
  data() {
    return {
      email: "",
      password: "",
    };
  },
  components: {},
  methods: {
    login() {
      // Handle login logic
      console.log("Email:", this.email, "Password:", this.password);
    },
  },
};
</script>

<style>
/* Add any additional custom styles here if needed */
.bg-auth-layout {
  background-image: url("/4.jpg");
}
</style>
