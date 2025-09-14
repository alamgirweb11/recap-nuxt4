<template>
  <div>
    <!-- Hero Section -->
    <section class="relative overflow-hidden">
      <!-- Background Elements -->
      <div class="absolute inset-0 bg-gradient-to-br from-blue-50 via-white to-purple-50 dark:from-gray-900 dark:via-gray-800 dark:to-purple-900/20"></div>
      <div class="absolute -top-40 -right-32 w-80 h-80 bg-gradient-to-r from-blue-400/30 to-purple-600/30 rounded-full blur-3xl"></div>
      <div class="absolute -bottom-40 -left-32 w-80 h-80 bg-gradient-to-r from-purple-400/30 to-pink-600/30 rounded-full blur-3xl"></div>

      <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-24 sm:py-32">
        <div class="text-center">
          <!-- Main Title -->
          <h1 class="text-4xl sm:text-6xl lg:text-7xl font-bold mb-6">
            <span class="bg-gradient-to-r from-gray-900 via-blue-800 to-purple-800 dark:from-white dark:via-blue-200 dark:to-purple-200 bg-clip-text text-transparent">
              Welcome to the
            </span>
            <br>
            <span class="bg-gradient-to-r from-blue-600 via-purple-600 to-pink-600 bg-clip-text text-transparent">
              Contact Page
            </span>
          </h1>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
// Page meta
useHead({
  title: 'Welcome to NuxtApp',
  meta: [
    { name: 'description', content: 'Modern web application built with Nuxt 4 and Tailwind CSS' }
  ]
})
</script>