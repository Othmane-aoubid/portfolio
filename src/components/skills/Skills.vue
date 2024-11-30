<template>
  <section class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
    <div class="space-y-8">
      <!-- Section Title -->
      <h2 class="text-4xl font-bold text-gray-900">Technical Skills</h2>

      <!-- Description -->
      <p class="text-lg text-gray-700 leading-relaxed">
        Othmane is proficient in a variety of <span class="text-blue-600">programming languages and frameworks</span>, including JavaScript, React, Node.js, and Python. His skills enable him to build robust and scalable web applications.
      </p>

      <!-- Skills Grid -->
      <div class="grid md:grid-cols-2 gap-8 mt-8">
        <!-- Front-End -->
        <div class="space-y-4">
          <h3 class="text-2xl font-bold text-gray-900">Front-End</h3>
          <p class="text-gray-700">
            Expertise in creating responsive and user-friendly interfaces using 
            <span class="text-blue-600">HTML, CSS</span>, and 
            <span class="text-blue-600">JavaScript</span> frameworks like 
            <span class="text-blue-600">React</span> and 
            <span class="text-blue-600">Vue.js</span>.
          </p>
        </div>

        <!-- Back-End -->
        <div class="space-y-4">
          <h3 class="text-2xl font-bold text-gray-900">Back-End</h3>
          <p class="text-gray-700">
            Skilled in server-side development with 
            <span class="text-blue-600">Node.js, Express</span>, and 
            <span class="text-blue-600">Python</span>, ensuring efficient data handling and application performance.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ComponentName',
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