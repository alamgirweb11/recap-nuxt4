<!-- layouts/default.vue -->
<template>
  <div class="min-h-screen bg-gradient-to-br from-slate-50 to-gray-100 dark:from-gray-900 dark:to-slate-800">
    <!-- Header -->
    <header class="backdrop-blur-md bg-white/80 dark:bg-gray-900/80 border-b border-gray-200/50 dark:border-gray-700/50 sticky top-0 z-50">
      <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex justify-between items-center h-16">
          <!-- Logo -->
          <div class="flex-shrink-0">
            <NuxtLink to="/" class="flex items-center space-x-2 group">
              <div class="w-8 h-8 bg-gradient-to-r from-blue-500 to-purple-600 rounded-lg flex items-center justify-center group-hover:scale-105 transition-transform duration-200">
                <span class="text-white font-bold text-sm">N</span>
              </div>
              <span class="text-xl font-bold bg-gradient-to-r from-gray-900 to-gray-700 dark:from-white dark:to-gray-300 bg-clip-text text-transparent">
                NuxtApp
              </span>
            </NuxtLink>
          </div>

          <!-- Navigation Links -->
          <div class="hidden md:block">
            <div class="ml-10 flex items-baseline space-x-8">
              <NuxtLink 
                to="/" 
                class="text-gray-700 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 px-3 py-2 rounded-md text-sm font-medium transition-colors duration-200 hover:bg-gray-100/50 dark:hover:bg-gray-800/50"
              >
                Home
              </NuxtLink>
              <NuxtLink 
                to="/about" 
                class="text-gray-700 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 px-3 py-2 rounded-md text-sm font-medium transition-colors duration-200 hover:bg-gray-100/50 dark:hover:bg-gray-800/50"
              >
                About
              </NuxtLink>
              <NuxtLink 
                to="/contact" 
                class="text-gray-700 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 px-3 py-2 rounded-md text-sm font-medium transition-colors duration-200 hover:bg-gray-100/50 dark:hover:bg-gray-800/50"
              >
                Contact
              </NuxtLink>
            </div>
          </div>

          <!-- Mobile menu button -->
          <div class="md:hidden">
            <button 
              @click="mobileMenuOpen = !mobileMenuOpen"
              class="text-gray-700 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 p-2 rounded-md transition-colors duration-200"
            >
              <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path v-if="!mobileMenuOpen" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                <path v-else stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
              </svg>
            </button>
          </div>
        </div>

        <!-- Mobile menu -->
        <div v-show="mobileMenuOpen" class="md:hidden">
          <div class="px-2 pt-2 pb-3 space-y-1 bg-white/90 dark:bg-gray-900/90 backdrop-blur-md rounded-lg mt-2 border border-gray-200/50 dark:border-gray-700/50">
            <NuxtLink 
              to="/" 
              class="block text-gray-700 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 px-3 py-2 rounded-md text-base font-medium transition-colors duration-200"
              @click="mobileMenuOpen = false"
            >
              Home
            </NuxtLink>
            <NuxtLink 
              to="/about" 
              class="block text-gray-700 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 px-3 py-2 rounded-md text-base font-medium transition-colors duration-200"
              @click="mobileMenuOpen = false"
            >
              About
            </NuxtLink>
            <NuxtLink 
              to="/contact" 
              class="block text-gray-700 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 px-3 py-2 rounded-md text-base font-medium transition-colors duration-200"
              @click="mobileMenuOpen = false"
            >
              Contact
            </NuxtLink>
          </div>
        </div>
      </nav>
    </header>

    <!-- Main Content -->
    <main class="flex-1">
      <slot />
    </main>

    <!-- Footer -->
    <footer class="bg-white/80 dark:bg-gray-900/80 backdrop-blur-md border-t border-gray-200/50 dark:border-gray-700/50">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
        <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
          <!-- Company Info -->
          <div class="col-span-1 md:col-span-2">
            <div class="flex items-center space-x-2 mb-4">
              <div class="w-8 h-8 bg-gradient-to-r from-blue-500 to-purple-600 rounded-lg flex items-center justify-center">
                <span class="text-white font-bold text-sm">N</span>
              </div>
              <span class="text-xl font-bold bg-gradient-to-r from-gray-900 to-gray-700 dark:from-white dark:to-gray-300 bg-clip-text text-transparent">
                NuxtApp
              </span>
            </div>
            <p class="text-gray-600 dark:text-gray-400 max-w-md">
              Building modern web applications with Nuxt.js and cutting-edge technologies. 
              Fast, secure, and beautifully designed.
            </p>
          </div>

          <!-- Quick Links -->
          <div>
            <h3 class="font-semibold text-gray-900 dark:text-white mb-4">Quick Links</h3>
            <ul class="space-y-2">
              <li>
                <NuxtLink to="/" class="text-gray-600 dark:text-gray-400 hover:text-blue-600 dark:hover:text-blue-400 transition-colors duration-200">
                  Home
                </NuxtLink>
              </li>
              <li>
                <NuxtLink to="/about" class="text-gray-600 dark:text-gray-400 hover:text-blue-600 dark:hover:text-blue-400 transition-colors duration-200">
                  About
                </NuxtLink>
              </li>
              <li>
                <NuxtLink to="/contact" class="text-gray-600 dark:text-gray-400 hover:text-blue-600 dark:hover:text-blue-400 transition-colors duration-200">
                  Contact
                </NuxtLink>
              </li>
            </ul>
          </div>

          <!-- Social Links -->
          <div>
            <h3 class="font-semibold text-gray-900 dark:text-white mb-4">Follow Us</h3>
            <div class="flex space-x-4">
              <a href="#" class="text-gray-600 dark:text-gray-400 hover:text-blue-600 dark:hover:text-blue-400 transition-colors duration-200">
                <span class="sr-only">Twitter</span>
                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                  <path d="M8.29 20.251c7.547 0 11.675-6.253 11.675-11.675 0-.178 0-.355-.012-.53A8.348 8.348 0 0022 5.92a8.19 8.19 0 01-2.357.646 4.118 4.118 0 001.804-2.27 8.224 8.224 0 01-2.605.996 4.107 4.107 0 00-6.993 3.743 11.65 11.65 0 01-8.457-4.287 4.106 4.106 0 001.27 5.477A4.072 4.072 0 012.8 9.713v.052a4.105 4.105 0 003.292 4.022 4.095 4.095 0 01-1.853.07 4.108 4.108 0 003.834 2.85A8.233 8.233 0 012 18.407a11.616 11.616 0 006.29 1.84" />
                </svg>
              </a>
              <a href="#" class="text-gray-600 dark:text-gray-400 hover:text-blue-600 dark:hover:text-blue-400 transition-colors duration-200">
                <span class="sr-only">GitHub</span>
                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                  <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z" />
                </svg>
              </a>
            </div>
          </div>
        </div>

        <!-- Bottom Section -->
        <div class="mt-8 pt-8 border-t border-gray-200 dark:border-gray-700">
          <p class="text-center text-gray-600 dark:text-gray-400">
            © {{ currentYear }} NuxtApp. All rights reserved.
          </p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
const mobileMenuOpen = ref(false)
const currentYear = new Date().getFullYear()

// Close mobile menu when route changes
const route = useRoute()
watch(() => route.path, () => {
  mobileMenuOpen.value = false
})
</script>