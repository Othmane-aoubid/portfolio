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
          <h1
            class="text-4xl sm:text-5xl md:text-6xl font-bold mb-8 relative inline-block"
          >
            <span class="relative z-10">Welcome to My Portfolio</span>
            <svg
              class="absolute bottom-0 left-0 w-full h-2"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 500 10"
              fill="none"
            >
              <path
                d="M0 5 H500"
                stroke="white"
                stroke-width="2"
                class="animate-twbb-dash"
              />
            </svg>
          </h1>

          <p class="text-lg sm:text-xl md:text-2xl text-gray-100 mb-12 text-justify font-bold">
            Hi, I’m Othmane ! A passionate Software Engineer with over two
            years of experience in building innovative web applications. I
            specialize in creating scalable, user-friendly solutions tailored to
            meet client needs. From collaborating with world-renowned
            organizations to delivering cutting-edge platforms, I turn ideas
            into reality with clean code and creative problem-solving. Let’s
            build something amazing together!
          </p>
          <div
            class="flex flex-col sm:flex-row justify-center space-y-4 sm:space-y-0 sm:space-x-6"
          >
            <router-link to="/projects">
              <button
                class="bg-white text-black px-8 py-3 rounded-md hover:bg-gray-200 transition-colors"
              >
                View Projects
              </button>
            </router-link>
            <router-link to="/contact">
            <button
            class="bg-white text-black px-9 py-3 rounded-md hover:bg-gray-200 transition-colors"
            >
               Contact Me 
            </button></router-link>
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
    <!-- Certificates Section -->
    <div class="bg-white">
      <CertificatesView />
    </div>
    <!-- Client Feed Back Section -->
    <!-- <div class="bg-white">
      <ClientFeedBack />
    </div> -->
    <!-- Insights Section -->
    <!-- <div class="bg-white">
      <Insights />
    </div> -->
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
import CertificatesView from "../views/CertificatesView.vue";
</script>

<style>
/* Add any custom styles here */
body {
  margin: 0;
  padding: 0;
}
</style>
