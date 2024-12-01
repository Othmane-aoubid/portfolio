<template>
  <section class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 sm:py-12">
    <div class="grid lg:grid-cols-2 gap-8 lg:gap-12 items-center">
      <!-- Left Content -->
      <div class="space-y-8">
        <!-- Bio Section -->
        <div class="space-y-4">
          <p class="text-base sm:text-lg text-gray-700 leading-relaxed">
            <span class="font-medium">Othmane</span> is a <span class="text-blue-600 font-medium">Full Stack Developer</span> with over two years of experience 
            in creating dynamic web applications. His expertise spans both front-end and back-end technologies, ensuring a seamless user experience 
            and robust functionality.
          </p>
        </div>

        <!-- Stats Grid -->
        <div class="grid grid-cols-1 sm:grid-cols-2 gap-6 sm:gap-8">
          <!-- Projects -->
          <div class="space-y-2">
            <h3 class="text-3xl sm:text-4xl font-bold text-gray-900">100 projects</h3>
            <p class="text-sm sm:text-base text-gray-600">
              Successfully completed numerous projects that showcase his ability to deliver practical solutions.
            </p>
          </div>

          <!-- Technologies -->
          <div class="space-y-2">
            <h3 class="text-3xl sm:text-4xl font-bold text-gray-900">50 technologies</h3>
            <p class="text-sm sm:text-base text-gray-600">
              Proficient in a variety of technologies, including JavaScript frameworks, which he uses to build scalable applications.
            </p>
          </div>

          <!-- Years -->
          <div class="space-y-2">
            <h3 class="text-3xl sm:text-4xl font-bold text-gray-900">10 years</h3>
            <p class="text-sm sm:text-base text-gray-600">
              Othmane is committed to continuous learning and improvement, always seeking to enhance his skills.
            </p>
          </div>

          <!-- Clients -->
          <div class="space-y-2">
            <h3 class="text-3xl sm:text-4xl font-bold text-gray-900">20 clients</h3>
            <p class="text-sm sm:text-base text-gray-600">
              He has collaborated with various clients, ensuring their needs are met with integrity and transparency.
            </p>
          </div>
        </div>
      </div>

      <!-- Right Image -->
      <div class="relative h-full rounded-2xl overflow-hidden mt-8 lg:mt-0">
        <img
          src="../../assets/images/second.webp"
          alt="Professional developer at work"
          class="w-full h-auto object-cover"
          style="max-height: 600px;"
        />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'AboutMe',
  data() {
    return {
      // component data here
    }
  },
  methods: {
    // component methods here
  }
}
</script>

<style scoped>
/* component styles here */
</style>

