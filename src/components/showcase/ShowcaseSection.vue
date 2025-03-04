<template>
  <section class="py-20 px-6 bg-[#0D1117]" style="border-top: 3px solid">
    <div class="max-w-7xl mx-auto">
      <h2 class="text-3xl font-semibold text-center mb-16 text-white relative">
        Recent Projects
        <div class="absolute bottom-0 left-1/2 transform -translate-x-1/2 w-16 h-1 bg-[#00FF95] mt-2"></div>
      </h2>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <!-- Predictive Platform -->
        <div class="bg-[#1A1F29] rounded-lg overflow-hidden">
          <img
            src="../../assets/images/predictive.png"
            alt="Predictive Platform"
            class="w-full h-48 object-cover"
          />
          <div class="p-6">
            <h3 class="text-xl font-semibold text-white mb-3">Predictive Platform</h3>
            <p class="text-gray-400 mb-4">Predictive is a security and vulnerability scanning platform that identifies and predicts security threats before they happen.</p>
            <div class="flex gap-2">
              <span class="inline-flex items-center px-3 py-1 rounded text-sm bg-[#00FF95]/20 text-[#00FF95]">
                Vue.js
              </span>
              <span class="inline-flex items-center px-3 py-1 rounded text-sm bg-[#00FF95]/20 text-[#00FF95]">
                Firebase
              </span>
              <span class="inline-flex items-center px-3 py-1 rounded text-sm bg-[#00FF95]/20 text-[#00FF95]">
                Flask
              </span>
            </div>
          </div>
        </div>

        <!-- Trident Platform -->
        <div class="bg-[#1A1F29] rounded-lg overflow-hidden">
          <img
            src="../../assets/images/TridentApp2.png"
            alt="Trident Platform"
            class="w-full h-48 object-cover"
          />
          <div class="p-6">
            <h3 class="text-xl font-semibold text-white mb-3">Trident Platform</h3>
            <p class="text-gray-400 mb-4">Energy optimization platform helping citizens sell unused electricity back to providers, developed in collaboration with Tisalabs and the Irish Government.</p>
            <div class="flex gap-2">
              <span class="inline-flex items-center px-3 py-1 rounded text-sm bg-[#00FF95]/20 text-[#00FF95]">
                Vue.js
              </span>
              <span class="inline-flex items-center px-3 py-1 rounded text-sm bg-[#00FF95]/20 text-[#00FF95]">
                Firebase
              </span>
              <span class="inline-flex items-center px-3 py-1 rounded text-sm bg-[#00FF95]/20 text-[#00FF95]">
                Flask
              </span>
            </div>
          </div>
        </div>

        <!-- OFZONE Agency -->
        <div class="bg-[#1A1F29] rounded-lg overflow-hidden">
          <img
            src="../../assets/images/Offzoneagency.png"
            alt="OFZONE Agency"
            class="w-full h-48 object-cover"
          />
          <div class="p-6">
            <h3 class="text-xl font-semibold text-white mb-3">OFZONE Agency Website</h3>
            <p class="text-gray-400 mb-4">A sleek, modern website optimized for fast loading times, SEO, and smooth user experience, built in collaboration with a team of developers.</p>
            <div class="flex gap-2">
              <span class="inline-flex items-center px-3 py-1 rounded text-sm bg-[#00FF95]/20 text-[#00FF95]">
                Next.js
              </span>
            </div>
          </div>
        </div>

        <!-- AutoWaysee Website -->
        <div class="bg-[#1A1F29] rounded-lg overflow-hidden">
          <img
            src="../../assets/images/autorepairshop.png"
            alt="AutoWaysee"
            class="w-full h-48 object-cover"
          />
          <div class="p-6">
            <h3 class="text-xl font-semibold text-white mb-3">AutoWaysee Website</h3>
            <p class="text-gray-400 mb-4">An e-commerce platform for car repair shops, enabling users to explore, purchase, and book automotive services and products online.</p>
            <div class="flex gap-2">
              <span class="inline-flex items-center px-3 py-1 rounded text-sm bg-[#00FF95]/20 text-[#00FF95]">
                Vue.js
              </span>
              <span class="inline-flex items-center px-3 py-1 rounded text-sm bg-[#00FF95]/20 text-[#00FF95]">
                Tailwind
              </span>
              <span class="inline-flex items-center px-3 py-1 rounded text-sm bg-[#00FF95]/20 text-[#00FF95]">
                Firebase
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ShowcaseSection"
}
</script>
