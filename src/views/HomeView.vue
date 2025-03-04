<template>
  <div class="min-h-screen">
    <!-- Hero Section -->
    <section class="relative h-screen flex items-center px-6">
      <div class="max-w-7xl mx-auto w-full">
        <div class="flex flex-col md:flex-row items-center justify-between">
          <!-- Left side content -->
          <div class="md:w-1/2">
            <h1 class="text-4xl md:text-5xl font-bold mb-4">
              Welcome to My
              <span class="text-[#00FF95]">Portfolio</span>
            </h1>
            <p class="text-gray-400 mb-8 max-w-lg">
              I'm a passionate developer specializing in web development, networking, and AI technologies.
            </p>
            <div class="flex gap-4">
              <router-link to="/projects" class="inline-block">
                <button class="bg-[#00B87C] text-white px-8 py-3 rounded-md hover:bg-[#00A06D] transition-colors font-medium">
                  View Projects
                </button>
              </router-link>
              <router-link to="/contact" class="inline-block">
                <button class="bg-[#0D1117] text-white px-8 py-3 rounded-md border border-[#1E2A3B] hover:border-[#2E3A4B] transition-colors font-medium">
                  Contact Me
                </button>
              </router-link>
            </div>
          </div>
          
          <!-- Right side with circular logo -->
          <div class="md:w-1/2 flex justify-center mt-12 md:mt-0">
            <div class="relative w-64 h-64">
              <div class="absolute inset-0 rounded-full bg-white glow-effect"></div>
              <div class="absolute inset-0 rounded-full overflow-hidden">
                <img 
                  src="../../public/hero.webp" 
                  alt="Hero Image" 
                  class="w-full h-full object-cover transform scale-110"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- About Me section will go here -->
    <div class="bg-white">
      <AboutMe />
    </div>
    <!-- Skills Section -->
    <div class="bg-white">
      <Skills />
    </div>
    <!-- Showcase Section -->
    <Showcase />
    <!-- Professional Journey Section -->
    <ProfessionalJourney />
    <!-- Certificates Section -->
    <!-- <div class="bg-white">
      <CertificatesView />
    </div> -->
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

<script>
import { ref } from "vue";
import AboutMe from "../components/about/AboutMe.vue";
import ProfessionalJourney from "../components/ProfessionalJourney/ProfessionalJourney.vue";
import Skills from "../components/skills/Skills.vue";
import Showcase from "../components/showcase/ShowcaseSection.vue";
import ClientFeedBack from "../components/clientfeedback/FeedBack.vue";
import Insights from "../components/insights/Insights.vue";
import CertificatesView from "../views/CertificatesView.vue";

export default {
  name: 'HomeView',
  components: {
    AboutMe,
    ProfessionalJourney,
    Skills,
    Showcase,
    ClientFeedBack,
    Insights,
    CertificatesView
  }
}
</script>

<style scoped>
.glow-effect {
  box-shadow: 0 0 40px 5px #00FF95;
}

.hero-gradient {
  background: linear-gradient(180deg, rgba(13,17,23,0) 0%, #0D1117 100%);
}
</style>
