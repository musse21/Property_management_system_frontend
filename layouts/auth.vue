<template>
  <div
    class="min-h-screen flex items-center justify-center bg-auth-layout bg-no-repeat"
  >
    <!-- bg-gradient-to-r from-blue-400 to-lightblue-400 -->
    <div class="max-w-md w-full bg-transparent rounded-lg p-8">
      <Nuxt />
    </div>
  </div>
</template>

<script>
export default {
  name: "AuthLayout",
};
</script>

<style>
.bg-auth-layout {
  background-image: url("/4.jpg");
  background-size: cover;
  background-position: center;
background-repeat: no-repeat;}
</style>
