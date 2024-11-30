<template>
  <section class="text-center py-16">
    <h2 class="text-lg font-semibold text-gray-800">OUR PROJECTS</h2>
    <h1 class="text-4xl font-bold text-gray-900">Showcasing My Work</h1>
    <p class="mt-2 text-lg text-gray-800">
      Explore a selection of my projects that demonstrate my skills in web
      development and design.
    </p>
    <div class="w-4/5 mx-9 mt-8 grid grid-cols-1 gap-8" style="width: 90% !important;">
      <div class="bg-white rounded-lg overflow-hidden">
        <img
          src="../../assets/images/project1.webp"
          alt="E-commerce Platform"
          class="w-full object-cover"
        />
        <div class="max-w-7xl mx-auto mt-5">
          <div class="grid grid-cols-2 gap-2">
            <!-- Left Column -->
            <div>
              <h1 class="text-3xl font-bold text-gray-900 mb-6 text-left">
                E-commerce Platform
              </h1>
              <div class="space-y-2 mb-8">
                <div class="flex items-center text-sm text-gray-600">
                  <span class="text-gray-400 mr-2">#</span>
                  <span>Client: Client: Online Retailer </span>
                </div>
                <div class="flex items-center text-sm text-gray-600">
                  <span class="text-gray-400 mr-2">#</span>
                  <span>Date: Date: May 2023 </span>
                </div>
                <div class="flex items-center text-sm text-gray-600">
                  <span class="text-gray-400 mr-2">#</span>
                  <span>Features: Features: User-friendly interface</span>
                </div>
              </div>
              <div class="mt-auto" style="text-align: left !important;">
                <a
                  href="#"
                  class="inline-flex items-center text-blue-600 hover:text-blue-800 "
                >
                  View Project
                  <svg
                    class="w-4 h-4 ml-1"
                    viewBox="0 0 24 24"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M9 5L16 12L9 19"
                      stroke="currentColor"
                      stroke-width="2"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                </a>
              </div>
            </div>

            <!-- Right Column -->
            <div class="flex items-center">
              <p class="text-gray-700 leading-relaxed">
                This e-commerce platform allows users to browse products, add
                them to a cart, and complete purchases securely. It features a
                robust back-end management system and a clean, user-friendly
                interface that enhances the shopping experience.
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="bg-white rounded-lg overflow-hidden">
        <img
          src="../../assets/images/project2.webp"
          alt="Personal Blog"
          class="w-full object-cover"
        />
        <div class="max-w-7xl mx-auto mt-5">
          <div class="grid grid-cols-2 gap-2">
            <!-- Left Column -->
            <div>
              <h1 class="text-3xl font-bold text-gray-900 mb-6 text-left">
                E-commerce Platform
              </h1>
              <div class="space-y-2 mb-8">
                <div class="flex items-center text-sm text-gray-600">
                  <span class="text-gray-400 mr-2">#</span>
                  <span>Client: Client: Online Retailer </span>
                </div>
                <div class="flex items-center text-sm text-gray-600">
                  <span class="text-gray-400 mr-2">#</span>
                  <span>Date: Date: May 2023 </span>
                </div>
                <div class="flex items-center text-sm text-gray-600">
                  <span class="text-gray-400 mr-2">#</span>
                  <span>Features: Features: User-friendly interface</span>
                </div>
              </div>
              <div class="mt-auto" style="text-align: left !important;">
                <a
                  href="#"
                  class="inline-flex items-center text-blue-600 hover:text-blue-800"
                >
                  View Project
                  <svg
                    class="w-4 h-4 ml-1"
                    viewBox="0 0 24 24"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M9 5L16 12L9 19"
                      stroke="currentColor"
                      stroke-width="2"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                </a>
              </div>
            </div>

            <!-- Right Column -->
            <div class="flex items-center">
              <p class="text-gray-700 leading-relaxed">
                This e-commerce platform allows users to browse products, add
                them to a cart, and complete purchases securely. It features a
                robust back-end management system and a clean, user-friendly
                interface that enhances the shopping experience.
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ShowcaseSection",
};
</script>

<style scoped>
/* Add any additional styles here if needed */
</style>
