<template>
  <div class="min-h-screen bg-black text-white">
    <!-- Hero Section -->
    <div class="relative min-h-screen flex items-center">
      <!-- Background Image -->
      <div class="absolute inset-0 z-0">
        <img
          src="../assets/images/hero.webp"
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
          <div
            class="flex flex-col sm:flex-row justify-center space-y-4 sm:space-y-0 sm:space-x-6"
          >
            <button
              class="bg-white text-black px-8 py-3 rounded-md hover:bg-gray-200 transition-colors"
            >
              View Projects
            </button>
            <button
              class="border border-white px-8 py-3 rounded-md hover:bg-white/10 transition-colors"
            >
              <router-link to="/contact"> Contact Me </router-link>
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
  </div>
</template>

<script setup>
import { ref } from "vue";
import AboutMe from "../components/about/AboutMe.vue";
import ProfessionalJourney from "../components/ProfessionalJourney/ProfessionalJourney.vue";
import Skills from "../components/skills/Skills.vue";
import Showcase from "../components/showcase/ShowcaseSection.vue";
import ClientFeedBack from "../components/clientfeedback/FeedBack.vue";
import Insights from "../components/insights/Insights.vue";
</script>

<style>
/* Add any custom styles here */
body {
  margin: 0;
  padding: 0;
}
</style>
