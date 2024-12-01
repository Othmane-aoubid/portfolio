<template>
  <div class="min-h-screen bg-black text-white">
    <!-- Navigation -->
    <nav class="fixed top-0 w-full bg-black/80 backdrop-blur-sm z-50">
      <div class="container mx-auto px-4">
        <div class="flex justify-between items-center h-16">
          <h1 class="text-2xl font-bold">
            <div class="h-14 rounded-2xl overflow-hidden">
              <img
                src="./assets/images/logo.webp"
                alt="Professional developer at work"
                class="w-full h-full object-cover"
                style="height:600;width:800"
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
            class="hidden md:block bg-white text-black px-6 py-2 rounded-md hover:bg-gray-200 transition-colors"
          >
            View Projects
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
        <a
          v-for="item in navItems"
          :key="item"
          :href="`#${item.toLowerCase().replace(' ', '-')}`"
          class="text-2xl hover:text-purple-400 transition-colors"
          @click="toggleMenu"
        >
          {{ item }}
        </a>
        <button
          class="bg-white text-black px-6 py-2 rounded-md hover:bg-gray-200 transition-colors"
          @click="toggleMenu"
        >
          View Projects
        </button>
      </div>
    </div>

    <!-- Rest of the content remains unchanged -->
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
          <h1 class="text-4xl sm:text-5xl md:text-6xl font-bold mb-8">
            Welcome to My Portfolio
          </h1>
          <p class="text-lg sm:text-xl md:text-2xl text-gray-300 mb-12">
            I am a passionate Full Stack Developer with over two years of
            experience in creating and optimizing modern web applications. Let's
            explore my skills and projects that showcase my expertise.
          </p>
          <div class="flex flex-col sm:flex-row justify-center space-y-4 sm:space-y-0 sm:space-x-6">
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
    <!-- Showcase Section -->
    <div class="bg-white">
      <Showcase />
    </div>
    <!-- Professional Journey Section -->
    <div class="bg-white">
      <ProfessionalJourney />
    </div>
    <!-- Client Feed Back Section -->
    <div class="bg-white">
      <ClientFeedBack />
    </div>
    <!-- Insights Section -->
    <div class="bg-white">
      <Insights />
    </div>
    <!-- footer Section -->
    <div class="bg-white">
      <Footer />
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import AboutMe from "./components/about/AboutMe.vue";
import ProfessionalJourney from "./components/ProfessionalJourney/ProfessionalJourney.vue";
import Skills from "./components/skills/Skills.vue";
import Showcase from "./components/showcase/ShowcaseSection.vue";
import ClientFeedBack from "./components/clientfeedback/FeedBack.vue";
import Insights from "./components/insights/Insights.vue";
import Footer from "./components/footer/Footer.vue";

const navItems = ["About Me", "Projects", "Experience", "Blog", "Contact Me"];
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