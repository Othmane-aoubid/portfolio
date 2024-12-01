<template>
  <section class="w-full bg-white py-20 md:px-20 lg:px-40" style="padding-inline: 4rem;">
    <h1 class="text-center text-2xl md:text-4xl font-bold text-gray-800 mb-10">About Othmane</h1>
    <p class="text-center text-gray-600 text-sm md:text-base mb-14">
      With over two years of experience, Othmane excels in both front-end and back-end development,
      delivering innovative web solutions that enhance user experience.
    </p>

    <div class="grid grid-cols-1 md:grid-cols-2 gap-10 items-center" >
      <!-- Left Section -->
      <div>
        <h2 class="text-xl md:text-2xl font-bold text-gray-800 mb-6">
          Othmane's Professional Journey
        </h2>
        <p class="text-gray-600 text-sm md:text-base mb-6">
          With over two years of experience, Othmane has honed his skills in both front-end and back-end development. 
          His expertise in JavaScript frameworks allows him to build efficient and scalable web applications that meet client needs.
        </p>

        <div class="grid grid-cols-2 gap-6">
          <!-- Achievements -->
          <div>
            <h3 class="text-lg font-bold text-gray-800">50 projects</h3>
            <p class="text-gray-600 text-sm md:text-base">
              Successfully completed projects that showcase his ability to deliver practical solutions.
            </p>
          </div>
          <div>
            <h3 class="text-lg font-bold text-gray-800">100 clients</h3>
            <p class="text-gray-600 text-sm md:text-base">
              Othmane has collaborated with numerous clients, ensuring their visions are brought to life through innovative web solutions.
            </p>
          </div>
          <div>
            <h3 class="text-lg font-bold text-gray-800">5 years</h3>
            <p class="text-gray-600 text-sm md:text-base">
              He is committed to continuous learning and improvement, always striving to enhance his skills and knowledge in the ever-evolving tech landscape.
            </p>
          </div>
          <div>
            <h3 class="text-lg font-bold text-gray-800">10 teams</h3>
            <p class="text-gray-600 text-sm md:text-base">
              Othmane values collaboration and teamwork, working effectively with cross-functional teams to achieve project goals.
            </p>
          </div>
        </div>
      </div>

      <!-- Right Section -->
      <div>
        <img
          src="../assets/images/media5.webp" 
          alt="Othmane's Professional Image" 
          class="rounded-lg shadow-lg"
          width="600px"
          height="600px"
        />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AboutMe",
};
</script>

<style scoped>
/* You can add custom styles here if needed */
</style>
