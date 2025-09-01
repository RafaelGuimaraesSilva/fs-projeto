<template>
  <div>
    <header class="bg-gray-900 text-white">
      <div class="container mx-auto px-6 py-3">
        <nav class="flex items-center justify-between">
          <div class="text-xl font-bold">
            Meu App
          </div>
          <div class="flex space-x-4">
            <NuxtLink to="/" class="hover:text-gray-300">Home</NuxtLink>
            <NuxtLink to="/login" class="hover:text-gray-300">Login</NuxtLink>
            <NuxtLink to="/register" class="hover:text-gray-300">Register</NuxtLink>
          </div>
        </nav>
      </div>
    </header>

    <main class="container mx-auto px-6 py-8">
      <NuxtPage />
    </main>
  </div>
</template>

<script setup>
// Component setup
</script>

<style>
/* Global styles */
</style>
