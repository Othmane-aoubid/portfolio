<template>
  <section class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 sm:py-12">
    <div class="grid lg:grid-cols-2 gap-8 lg:gap-12 items-center">
      <!-- Left Content -->
      <div class="space-y-6 sm:space-y-8">
        <h1
          class="text-2xl sm:text-3xl font-bold text-gray-900 mb-4 sm:mb-6 text-left"
        >
          Professional Journey
        </h1>
        <!-- Bio Section -->
        <div class="space-y-4">
          <p class="text-base sm:text-lg text-gray-700 leading-relaxed">
            <span class="font-medium">The journey </span> of a
            <span class="text-blue-600 font-medium">software engineer</span>
            is a path of continuous growth, creativity, and innovation. It
            begins with curiosity and evolves through mastering coding,
            debugging, and building complex systems. Along the way, the engineer
            achieves milestones like successful product launches, team
            collaborations, and contributions to transformative technologies.
            Each step involves adapting to new tools, solving real-world
            problems, and embracing lifelong learning. Beyond technical
            achievements, the journey is about creating meaningful
            change crafting solutions that impact lives, drive progress, and
            shape the future through the power of technology. At its core, this
            journey is fueled by passion and resilience. Each challenge, from
            debugging elusive errors to adapting to industry shifts, hones the
            engineer's skills and mindset. The professional timeline weaves
            together moments of collaboration, innovation, and inspiration,
            building a career that thrives on curiosity and purpose. Ultimately,
            the software engineer’s journey is not just about writing code—it’s
            about creating impact, connecting ideas, and leaving a lasting
            legacy in a digitally driven world.
          </p>
        </div>

        <!-- Stats Grid -->
      </div>

      <!-- Right Image -->
      <div class="relative h-full rounded-2xl overflow-hidden mt-8 lg:mt-0">
        <img
          src="../../assets/images/personaljourney.webp"
          alt="Professional developer at work"
          class="w-full h-auto object-cover"
          style="max-height: 600px"
        />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ProfessionalJourney",
  data() {
    return {
      // component data here
    };
  },
  methods: {
    // component methods here
  },
};
</script>

<style scoped>
/* component styles here */
</style>
