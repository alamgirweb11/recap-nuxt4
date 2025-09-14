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
              Future of Web
            </span>
          </h1>

          <!-- Subtitle -->
          <p class="text-xl sm:text-2xl text-gray-600 dark:text-gray-300 max-w-3xl mx-auto mb-12 leading-relaxed">
            Built with <strong class="text-emerald-600 dark:text-emerald-400">Nuxt 4</strong> and 
            <strong class="text-sky-600 dark:text-sky-400">Tailwind CSS</strong>. 
            Experience blazing-fast performance with modern design principles.
          </p>

          <!-- CTA Buttons -->
          <div class="flex flex-col sm:flex-row gap-4 justify-center items-center mb-16">
            <button class="group relative overflow-hidden bg-gradient-to-r from-blue-600 to-purple-600 text-white px-8 py-4 rounded-full font-semibold text-lg transition-all duration-300 hover:shadow-2xl hover:shadow-blue-500/25 hover:scale-105">
              <span class="relative z-10">Get Started</span>
              <div class="absolute inset-0 bg-gradient-to-r from-purple-600 to-pink-600 opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
            </button>
            
            <button class="group px-8 py-4 rounded-full border-2 border-gray-300 dark:border-gray-600 text-gray-700 dark:text-gray-300 font-semibold text-lg hover:border-blue-500 dark:hover:border-blue-400 hover:text-blue-600 dark:hover:text-blue-400 transition-all duration-300 hover:shadow-lg">
              Learn More
            </button>
          </div>

          <!-- Feature Cards -->
          <div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-5xl mx-auto">
            <!-- Feature 1 -->
            <div class="group p-8 bg-white/70 dark:bg-gray-800/70 backdrop-blur-sm rounded-2xl border border-gray-200/50 dark:border-gray-700/50 hover:shadow-xl hover:shadow-blue-500/10 transition-all duration-300 hover:-translate-y-2">
              <div class="w-12 h-12 bg-gradient-to-r from-blue-500 to-blue-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
                <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
                </svg>
              </div>
              <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-4">Lightning Fast</h3>
              <p class="text-gray-600 dark:text-gray-400">
                Built with Nuxt 4's cutting-edge architecture for unparalleled performance and user experience.
              </p>
            </div>

            <!-- Feature 2 -->
            <div class="group p-8 bg-white/70 dark:bg-gray-800/70 backdrop-blur-sm rounded-2xl border border-gray-200/50 dark:border-gray-700/50 hover:shadow-xl hover:shadow-purple-500/10 transition-all duration-300 hover:-translate-y-2">
              <div class="w-12 h-12 bg-gradient-to-r from-purple-500 to-purple-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
                <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 21a4 4 0 01-4-4V5a2 2 0 012-2h4a2 2 0 012 2v12a4 4 0 01-4 4zM21 5a2 2 0 00-2-2h-4a2 2 0 00-2 2v12a4 4 0 004 4h4a2 2 0 002-2V5z" />
                </svg>
              </div>
              <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-4">Responsive Design</h3>
              <p class="text-gray-600 dark:text-gray-400">
                Perfectly crafted interfaces that look stunning on every device, from mobile to desktop.
              </p>
            </div>

            <!-- Feature 3 -->
            <div class="group p-8 bg-white/70 dark:bg-gray-800/70 backdrop-blur-sm rounded-2xl border border-gray-200/50 dark:border-gray-700/50 hover:shadow-xl hover:shadow-emerald-500/10 transition-all duration-300 hover:-translate-y-2">
              <div class="w-12 h-12 bg-gradient-to-r from-emerald-500 to-emerald-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
                <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
                </svg>
              </div>
              <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-4">Modern Stack</h3>
              <p class="text-gray-600 dark:text-gray-400">
                Powered by the latest technologies including Vue 3, TypeScript, and modern build tools.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Stats Section -->
    <section class="py-20 bg-gradient-to-r from-gray-50 to-gray-100 dark:from-gray-800 dark:to-gray-900">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-1 md:grid-cols-4 gap-8 text-center">
          <div>
            <div class="text-4xl font-bold text-blue-600 dark:text-blue-400 mb-2">99.9%</div>
            <div class="text-gray-600 dark:text-gray-400">Uptime</div>
          </div>
          <div>
            <div class="text-4xl font-bold text-purple-600 dark:text-purple-400 mb-2">10k+</div>
            <div class="text-gray-600 dark:text-gray-400">Happy Users</div>
          </div>
          <div>
            <div class="text-4xl font-bold text-emerald-600 dark:text-emerald-400 mb-2">24/7</div>
            <div class="text-gray-600 dark:text-gray-400">Support</div>
          </div>
          <div>
            <div class="text-4xl font-bold text-pink-600 dark:text-pink-400 mb-2">50ms</div>
            <div class="text-gray-600 dark:text-gray-400">Response Time</div>
          </div>
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