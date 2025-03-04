<template>
  <section class="py-20 px-6 bg-[#0D1117]" style="border-top: 3px solid">
    <div class="max-w-7xl mx-auto">
      <h2 class="text-3xl font-semibold text-center mb-16 text-white relative">
        Professional Certifications
        <div class="absolute bottom-0 left-1/2 transform -translate-x-1/2 w-16 h-1 bg-[#00FF95] mt-2"></div>
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <!-- Networking Essentials -->
        <div class="bg-[#1A1F29] rounded-lg p-6">
          <div class="flex items-center gap-3 mb-4">
            <div class="w-8 h-8 rounded-full bg-[#00FF95]/20 flex items-center justify-center">
              <svg class="w-4 h-4 text-[#00FF95]" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
              </svg>
            </div>
            <h3 class="text-white text-lg font-medium">Networking Essentials</h3>
          </div>
          <p class="text-gray-400 mb-4">Cisco Networking Academy</p>
          <div class="flex justify-between items-center">
            <router-link :to="{ name: 'certificates', params: { file: 'Networking_Essentials_certificate_o_aoubid-etu-enset-media-ac-ma_63d735e0-2607-4452-8c2b-002c29508430.pdf' }}" class="text-[#00FF95] hover:text-[#00FF95]/80">View Certificate</router-link>
          </div>
        </div>

        <!-- Linux Essentials -->
        <div class="bg-[#1A1F29] rounded-lg p-6">
          <div class="flex items-center gap-3 mb-4">
            <div class="w-8 h-8 rounded-full bg-[#00FF95]/20 flex items-center justify-center">
              <svg class="w-4 h-4 text-[#00FF95]" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
              </svg>
            </div>
            <h3 class="text-white text-lg font-medium">Linux Essentials</h3>
          </div>
          <p class="text-gray-400 mb-4">NDG Linux</p>
          <div class="flex justify-between items-center">
            <router-link :to="{ name: 'certificates', params: { file: 'aoubidothmane-certificate-LINUX ESSENTIALS.pdf' }}" class="text-[#00FF95] hover:text-[#00FF95]/80">View Certificate</router-link>
          </div>
        </div>

        <!-- Linux Unhatched -->
        <div class="bg-[#1A1F29] rounded-lg p-6">
          <div class="flex items-center gap-3 mb-4">
            <div class="w-8 h-8 rounded-full bg-[#00FF95]/20 flex items-center justify-center">
              <svg class="w-4 h-4 text-[#00FF95]" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
              </svg>
            </div>
            <h3 class="text-white text-lg font-medium">NDG Linux Unhatched</h3>
          </div>
          <p class="text-gray-400 mb-4">NDG Linux</p>
          <div class="flex justify-between items-center">
            <router-link :to="{ name: 'certificates', params: { file: 'Partner-_NDG_Linux_Unhatched_certificate_o_aoubid-etu-enset-media-ac-ma_b77d576a-16fa-4297-ab42-b77633b5036c.pdf' }}" class="text-[#00FF95] hover:text-[#00FF95]/80">View Certificate</router-link>
          </div>
        </div>

        <!-- English for IT -->
        <div class="bg-[#1A1F29] rounded-lg p-6">
          <div class="flex items-center gap-3 mb-4">
            <div class="w-8 h-8 rounded-full bg-[#00FF95]/20 flex items-center justify-center">
              <svg class="w-4 h-4 text-[#00FF95]" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
              </svg>
            </div>
            <h3 class="text-white text-lg font-medium">English for IT</h3>
          </div>
          <p class="text-gray-400 mb-4">Cisco Networking Academy</p>
          <div class="flex justify-between items-center">
            <router-link :to="{ name: 'certificates', params: { file: 'English_for_IT_1_certificate_o_aoubid-etu-enset-media-ac-ma_36946776-5e5f-4131-a695-3f7b895b7656.pdf' }}" class="text-[#00FF95] hover:text-[#00FF95]/80">View Certificate</router-link>
          </div>
        </div>

        <!-- Introduction to IoT -->
        <div class="bg-[#1A1F29] rounded-lg p-6">
          <div class="flex items-center gap-3 mb-4">
            <div class="w-8 h-8 rounded-full bg-[#00FF95]/20 flex items-center justify-center">
              <svg class="w-4 h-4 text-[#00FF95]" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
              </svg>
            </div>
            <h3 class="text-white text-lg font-medium">Introduction to IoT</h3>
          </div>
          <p class="text-gray-400 mb-4">Cisco Networking Academy</p>
          <div class="flex justify-between items-center">
            <router-link :to="{ name: 'certificates', params: { file: 'Introduction_to_IoT_certificate_o_aoubid-etu-enset-media-ac-ma_e272b145-044d-48d8-8aee-c27ba8e801a7.pdf' }}" class="text-[#00FF95] hover:text-[#00FF95]/80">View Certificate</router-link>
          </div>
        </div>

        <!-- Principles of Cybersecurity -->
        <div class="bg-[#1A1F29] rounded-lg p-6">
          <div class="flex items-center gap-3 mb-4">
            <div class="w-8 h-8 rounded-full bg-[#00FF95]/20 flex items-center justify-center">
              <svg class="w-4 h-4 text-[#00FF95]" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
              </svg>
            </div>
            <h3 class="text-white text-lg font-medium">Principles of Cybersecurity</h3>
          </div>
          <p class="text-gray-400 mb-4">Cisco Networking Academy</p>
          <div class="flex justify-between items-center">
            <span class="text-gray-400">2025</span>
            <router-link :to="{ name: 'certificates', params: { file: '_certificate_o_aoubid-Principles-of- Cybersecurity.pdf' }}" class="text-[#00FF95] hover:text-[#00FF95]/80">View Certificate</router-link>
          </div>
        </div>

        <!-- Intro to ChatGPT -->
        <div class="bg-[#1A1F29] rounded-lg p-6">
          <div class="flex items-center gap-3 mb-4">
            <div class="w-8 h-8 rounded-full bg-[#00FF95]/20 flex items-center justify-center">
              <svg class="w-4 h-4 text-[#00FF95]" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
              </svg>
            </div>
            <h3 class="text-white text-lg font-medium">Intro to ChatGPT and Generative AI</h3>
          </div>
          <p class="text-gray-400 mb-4">OpenAI</p>
          <div class="flex justify-between items-center">
            <router-link :to="{ name: 'certificates', params: { file: 'othamen-Intro to ChatGPT and Generative AI.pdf' }}" class="text-[#00FF95] hover:text-[#00FF95]/80">View Certificate</router-link>
          </div>
        </div>

        <!-- Build Chat Applications -->
        <div class="bg-[#1A1F29] rounded-lg p-6">
          <div class="flex items-center gap-3 mb-4">
            <div class="w-8 h-8 rounded-full bg-[#00FF95]/20 flex items-center justify-center">
              <svg class="w-4 h-4 text-[#00FF95]" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
              </svg>
            </div>
            <h3 class="text-white text-lg font-medium">Build Chat Applications with OpenAI</h3>
          </div>
          <p class="text-gray-400 mb-4">OpenAI</p>
          <div class="flex justify-between items-center">
            <router-link :to="{ name: 'certificates', params: { file: 'othmane-Build Chat Applications with OpenAI.pdf' }}" class="text-[#00FF95] hover:text-[#00FF95]/80">View Certificate</router-link>
          </div>
        </div>

        <!-- Convolutional Neural Networks -->
        <div class="bg-[#1A1F29] rounded-lg p-6">
          <div class="flex items-center gap-3 mb-4">
            <div class="w-8 h-8 rounded-full bg-[#00FF95]/20 flex items-center justify-center">
              <svg class="w-4 h-4 text-[#00FF95]" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
              </svg>
            </div>
            <h3 class="text-white text-lg font-medium">Convolutional Neural Networks</h3>
          </div>
          <p class="text-gray-400 mb-4">TensorFlow</p>
          <div class="flex justify-between items-center">
            <router-link :to="{ name: 'certificates', params: { file: 'othmane-Convolutional Neural Networks with.pdf' }}" class="text-[#00FF95] hover:text-[#00FF95]/80">View Certificate</router-link>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ProfessionalJourney"
}
</script>
