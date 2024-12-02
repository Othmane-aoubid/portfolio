<template>
  <footer class="bg-white text-center py-6 sm:py-9">
    <div class="flex flex-col sm:flex-row justify-center items-center space-y-4 sm:space-y-0 sm:space-x-4">
      <div class="h-14 rounded-2xl overflow-hidden">
        <img
          src="../../assets/images/logo_vAJ5f7k2.webp?height=600&width=800"
          alt="Professional developer at work"
          class="w-full h-full object-cover"
        />
      </div>
      <nav class="flex flex-wrap justify-center space-x-4">
        <router-link to="/about" class="text-gray-600 hover:text-blue-500 py-2">About Me</router-link>
        <router-link to="/projects" class="text-gray-600 hover:text-blue-500 py-2">Projects</router-link>
        <router-link to="/experience" class="text-gray-600 hover:text-blue-500 py-2">Experience</router-link>
        <router-link to="/blog" class="text-gray-600 hover:text-blue-500 py-2">Blog</router-link>
        <router-link to="/contact" class="text-gray-600 hover:text-blue-500 py-2">Contact Me</router-link>
      </nav>
    </div>
    <hr class="my-6 sm:my-8" />
    <div class="text-gray-500 text-sm px-4">
      <p class="mb-2">© 2024 Othmane. All rights reserved.</p>
      <!-- <div class="space-x-2">
        <router-link to="/privacy" class="text-gray-500 hover:text-blue-500">Privacy Policy</router-link>
        <span class="text-gray-400">|</span>
        <router-link to="/terms" class="text-gray-500 hover:text-blue-500">Terms Of Service</router-link>
      </div> -->
    </div>
  </footer>
</template>

<script setup>
// No additional script needed for this component
</script>

<style scoped>
/* Add any custom styles here if needed */
</style>