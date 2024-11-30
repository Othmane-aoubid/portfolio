<template>
  <div class="min-h-screen bg-black text-white">
    <!-- Navigation -->
    <nav class="fixed top-0 w-full bg-black/80 backdrop-blur-sm z-50">
      <div class="container mx-auto px-4">
        <div class="flex justify-between items-center h-16">
          <h1 class="text-2xl font-bold">
            <div class="h-14 rounded-2xl overflow-hidden">
              <img
                src="./assets/images/logo.webp?height=600&width=800"
                alt="Professional developer at work"
                class="w-full h-full object-cover"
              />
            </div>
          </h1>
          <div class="hidden md:flex space-x-8">
            <a
              v-for="item in navItems"
              :key="item"
              :href="`#${item.toLowerCase().replace(' ', '-')}`"
              class="hover:text-purple-400 transition-colors"
            >
              {{ item }}
            </a>
          </div>
          <button
            class="bg-white text-black px-6 py-2 rounded-md hover:bg-gray-200 transition-colors"
          >
            View Projects
          </button>
        </div>
      </div>
    </nav>

    <!-- Hero Section -->
    <div class="relative min-h-screen flex items-center">
      <!-- Background Image -->
      <div class="absolute inset-0 z-0">
        <img
          src="./assets/images/hero.webp"
          alt="Cyberpunk cityscape"
          class="w-full h-full object-cover"
        />
        <div class="absolute inset-0 bg-black/50"></div>
      </div>

      <!-- Content -->
      <div class="relative z-10 container mx-auto px-4">
        <div class="max-w-3xl mx-auto text-center">
          <h1 class="text-5xl md:text-6xl font-bold mb-8">
            Welcome to My Portfolio
          </h1>
          <p class="text-xl md:text-2xl text-gray-300 mb-12">
            I am a passionate Full Stack Developer with over two years of
            experience in creating and optimizing modern web applications. Let's
            explore my skills and projects that showcase my expertise.
          </p>
          <div class="flex justify-center space-x-6">
            <button
              class="bg-white text-black px-8 py-3 rounded-md hover:bg-gray-200 transition-colors"
            >
              View Projects
            </button>
            <button
              class="border border-white px-8 py-3 rounded-md hover:bg-white/10 transition-colors"
            >
              Contact Me
            </button>
          </div>
        </div>
      </div>
    </div>
    <!-- about me Section -->
    <div class="bg-white">
      <AboutMe />
    </div>
    <!-- Skills Section -->
    <div class="bg-white">
      <Skills />
    </div>
  </div>
</template>

<script setup>
import AboutMe from "./components/about/AboutMe.vue";
import Skills from "./components/skills/Skills.vue";
const navItems = ["About Me", "Projects", "Experience", "Blog", "Contact Me"];
</script>

<style>
/* Add any custom styles here */
body {
  margin: 0;
  padding: 0;
}
</style>
