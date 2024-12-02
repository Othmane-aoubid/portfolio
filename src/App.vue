<template>
  <div class="min-h-screen bg-black text-white">
    <!-- Navigation -->
    <nav class="fixed top-0 w-full bg-black/80 backdrop-blur-sm z-50">
      <div class="container mx-auto px-4">
        <div class="flex justify-between items-center h-16">
          <h1 class="text-2xl font-bold">
            <div class="h-14 rounded-2xl overflow-hidden">
              <router-link to="/">
                <img
                  src="./assets/images/logo.webp"
                  alt="Professional developer at work"
                  class="w-full h-full object-cover"
                  style="height: 600; width: 800"
                />
              </router-link>
            </div>
          </h1>
          <div class="hidden md:flex space-x-8">
            <router-link
              v-for="item in navItems"
              :key="item.path"
              :to="item.path"
              class="hover:text-purple-400 transition-colors"
            >
              {{ item.label }}
            </router-link>
          </div>
          <button
            class="hidden md:block bg-white text-black px-6 py-2 rounded-md hover:bg-gray-200 transition-colors"
          >
            <router-link to="/projects">View Projects</router-link>
          </button>
          <!-- Hamburger menu button -->
          <button
            @click="toggleMenu"
            class="md:hidden text-white focus:outline-none"
          >
            <svg
              class="w-6 h-6"
              fill="none"
              stroke="currentColor"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16m-7 6h7"
              ></path>
            </svg>
          </button>
        </div>
      </div>
    </nav>
    <!-- Mobile menu -->
    <div
      v-show="isMenuOpen"
      class="md:hidden fixed inset-0 bg-black/95 z-40 flex flex-col items-center justify-center"
    >
      <button
        @click="toggleMenu"
        class="absolute top-4 right-4 text-white focus:outline-none"
      >
        <svg
          class="w-6 h-6"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M6 18L18 6M6 6l12 12"
          ></path>
        </svg>
      </button>
      <div class="flex flex-col items-center space-y-6">
        <router-link
          v-for="item in navItems"
          :key="item.path"
          :to="item.path"
          class="text-2xl hover:text-purple-400 transition-colors"
          @click="toggleMenu"
        >
          {{ item.label }}
        </router-link >
        <router-link to="/projects">
        <button
          class="bg-white text-black px-6 py-2 rounded-md hover:bg-gray-200 transition-colors"
          @click="toggleMenu"
        >
          View Projects
        </button></router-link>
      </div>
    </div>
    <!-- about me Section -->
    <div class="bg-white">
      <router-view />
    </div>
    <!-- footer Section -->
    <div class="bg-white">
      <Footer />
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
import Footer from "./components/footer/Footer.vue";

const navItems = [
  { label: "About Me", path: "/about" },
  { label: "Projects", path: "/projects" },
  { label: "Experience", path: "/experience" },
  { label: "Blog", path: "/blog" },
  { label: "Contact Me", path: "/contact" },
];
const isMenuOpen = ref(false);

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};
</script>

<style>
/* Add any custom styles here */
body {
  margin: 0;
  padding: 0;
}
</style>
