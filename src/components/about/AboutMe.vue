<template>
  <section class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 sm:py-12">
    <div class="grid lg:grid-cols-2 gap-8 lg:gap-12 items-center">
      <!-- Left Content -->
      <div class="space-y-8">
        <!-- Bio Section -->
        <div class="space-y-4">
          <h2 class="text-xl md:text-2xl font-bold text-gray-800 mb-6">
            About Me
          </h2>
          <p class="text-base sm:text-lg text-gray-700 leading-relaxed">
            <span class="font-medium">I’m a Software Engineer </span>
            <span class="text-blue-600 font-medium"
              >with expertise in front-end and back-end development.</span
            >
            Over the last two years, I’ve had the privilege of working on
            impactful projects in industries like sports, cybersecurity, and
            energy optimization. My passion lies in solving complex problems,
            collaborating with talented teams, and delivering software solutions
            that make a difference.
          </p>
        </div>

        <!-- Stats Grid -->
        <div class="grid grid-cols-1 sm:grid-cols-2 gap-6 sm:gap-8">
          <!-- Projects -->
          <div class="space-y-2">
            <h3 class="text-1xl sm:text-2xl font-bold text-gray-900">
              +5 projects
            </h3>
            <p class="text-sm sm:text-base text-gray-600">
              Crafted and delivered impactful solutions through 5+ successful
              projects, ranging from real-time data logging applications to
              energy optimization platforms.
            </p>
          </div>

          <!-- Technologies -->
          <div class="space-y-2">
            <h3 class="text-1xl sm:text-2xl font-bold text-gray-900">
              +10 technologies
            </h3>
            <p class="text-sm sm:text-base text-gray-600">
              Mastered over 10 cutting-edge technologies to build modern, robust
              applications. From versatile JavaScript frameworks like React.js,
              Vue.js, and Next.js to back-end powerhouses like Python Flask and
              Node.js.
            </p>
          </div>

          <!-- Years -->
          <div class="space-y-2">
            <h3 class="text-1xl sm:text-2xl font-bold text-gray-900">
              +3 years
            </h3>
            <p class="text-sm sm:text-base text-gray-600">
              With 3+ years of experience, I’m continuously learning, growing,
              and refining my skills to stay ahead of the curve.
            </p>
          </div>

          <!-- Clients -->
          <div class="space-y-2">
            <h3 class="text-1xl sm:text-2xl font-bold text-gray-900">
              4 clients
            </h3>
            <p class="text-sm sm:text-base text-gray-600">
              Collaborated with 4 esteemed clients, including organizations like
              the Royal Moroccan Football Federation and the Irish Government.
            </p>
          </div>
        </div>
      </div>

      <!-- Right Image -->
      <div class="relative h-full rounded-2xl overflow-hidden mt-8 lg:mt-0">
        <img
          src="../../assets/images/othmaneaoubid.jpg"
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
  name: "AboutMe",
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
