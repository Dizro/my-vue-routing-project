<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header class="bg-gray-800 text-white p-4">
    <div class="container mx-auto">
      <nav class="flex space-x-4">
        <RouterLink to="/" class="hover:bg-gray-700 px-3 py-2 rounded-md">Домой</RouterLink>
        <RouterLink to="/about" class="hover:bg-gray-700 px-3 py-2 rounded-md">О нас</RouterLink>
        <RouterLink to="/services" class="hover:bg-gray-700 px-3 py-2 rounded-md">Услуги</RouterLink>
        <RouterLink to="/contact" class="hover:bg-gray-700 px-3 py-2 rounded-md">Контакты</RouterLink>
      </nav>
    </div>
  </header>

  <main class="container mx-auto p-4">
    <RouterView />
  </main>

  <footer class="bg-gray-200 text-center p-4 mt-8">
    <p>&copy; 2025 Мое Vue Приложение</p>
  </footer>
</template>

<style scoped>
nav a.router-link-exact-active {
  background-color: #4a5568; /* bg-gray-700 */
  color: white;
}
</style>
