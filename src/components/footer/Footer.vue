<template>
  <footer class="bg-white text-center py-9">
    <div class="flex justify-center align-middle space-x-4">
      <div class="h-14 rounded-2xl overflow-hidden">
        <img
          src="../../assets/images/logo_vAJ5f7k2.webp?height=600&width=800"
          alt="Professional developer at work"
          class="w-full h-full object-cover"
        />
      </div>
      <nav class="flex space-x-4" style="display: flex; align-items: center; justify-content: center;">
        <router-link to="/about" class="text-gray-600 hover:text-blue-500 align-middle"
          >About Me</router-link
        >
        <router-link to="/projects" class="text-gray-600 hover:text-blue-500 align-middle"
          >Projects</router-link
        >
        <router-link to="/experience" class="text-gray-600 hover:text-blue-500 align-middle"
          >Experience</router-link
        >
        <router-link to="/blog" class="text-gray-600 hover:text-blue-500 align-middle"
          >Blog</router-link
        >
      </nav>
    </div>
    <hr class="my-8" />
    <div class="text-gray-500 text-sm">
      © 2024 Othmane. All rights reserved.
      <router-link to="/privacy" class="text-gray-500 hover:text-blue-500"
        >Privacy Policy</router-link
      >
      |
      <router-link to="/terms" class="text-gray-500 hover:text-blue-500"
        >Terms Of Service</router-link
      >
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped></style>
