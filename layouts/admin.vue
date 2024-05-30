<template>
    <div class="min-h-screen flex">
        <!--sidebar-->
        <aside class="w-64 bg-gray-800 text-white">
            <div class="p-4">
                <h2 class="text-2xl font-bold">Admin Pannel</h2>
            </div>

            <nav class="mt-8">
                <ul>
                    <li class="px-4 py-2 hover:bg-gray-700">
                        <nuxt-link to="/admin/dashboard" class="block">Dashboard</nuxt-link>
                    </li>
                    <li class="px-4 py-2 hover:bg-gray-700">
                        <nuxt-link to="/admin/users" class="block">Users</nuxt-link>
                    </li>
                    <li class="px-4 py-2 hover:bg-gray-700">
                        <nuxt-link to="/admin/settings" class="block">Settings</nuxt-link>
                    </li>
                </ul>
            </nav>
        </aside>
        <div class="flex-1 bg-gray-100 p-8">
            <div class="bg-gray-700 text-white box-border rounded-md shadow-lg px-1"><nuxt /></div>
            <div class="text-red-600 text-center">
                this is another content to be loaded
            </div>
        </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'AdminLayout'
  }
  </script>

<div class="min-h-screen flex items-center justify-center bg-gray-100">
    <div class="max-w-md w-full bg-white shadow-md rounded-lg p-8">
      <Nuxt />
    </div>
  </div>
  