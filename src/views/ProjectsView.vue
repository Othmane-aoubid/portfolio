<template>
  <section class="bg-white py-20 px-5 md:px-20 lg:px-40">
    <!-- Title -->
    <div class="text-center mb-10">
      <h1 class="text-2xl md:text-4xl font-bold text-gray-800 mb-4">Featured Projects</h1>
      <p class="text-gray-600 text-sm md:text-base">
        Explore a selection of standout projects, showcasing expertise in web development. Each project reflects my commitment to quality and innovation.
      </p>
    </div>

    <!-- Project List -->
    <div class="space-y-10">
      <!-- Single Project -->
      <div class="flex flex-col md:flex-row items-start md:items-center gap-6 border-b pb-10">
        <div class="flex-1">
          <h2 class="text-lg md:text-xl font-bold text-gray-800 mb-2">Predictive is a security and vulnerability scanning platform</h2>
          <p class="text-gray-600 text-sm md:text-base mb-4">
            Predictive is a security and vulnerability scanning platform that
            identifies and predicts security threats before they happen.
            Predictive was designed by a team of security experts who are
            passionate about developing better ways to protect organizations
            from Cyberattacks.
          </p>
          <p class="text-gray-500 text-sm">
            <span class="font-bold">Company:</span> Tisalabs &nbsp;&nbsp; | &nbsp;&nbsp;
            <span class="font-bold">Technologies:</span> Vue.js, Firebase, Python Flask
          </p>
          <a href="#" class="text-blue-500 text-sm underline mt-2 inline-block">Check Project →</a>
        </div>
        <img
          src="../assets/images/predictive.png"
          alt="Epredictive"
          class="rounded-lg shadow-lg w-full md:w-1/3"
          style="height: 150px ;"
        />
      </div>

      <!-- Second Project -->
      <div class="flex flex-col md:flex-row items-start md:items-center gap-6 border-b pb-10">
        <div class="flex-1">
          <h2 class="text-lg md:text-xl font-bold text-gray-800 mb-2">rident – Energy Usage Optimization Platform</h2>
          <p class="text-gray-600 text-sm md:text-base mb-4">
            Collaboration: Tisalabs and the Irish Government Trident is an
            energy optimization platform developed in collaboration with
            Tisalabs and the Irish Government. It helps citizens sell unused
            electricity back to providers, who can redistribute it to others in
            need. My role involved developing the front-end with Vue.js,
            creating back-end APIs with Python Flask, and managing data with
            Firebase to ensure seamless functionality.
          </p>
          <p class="text-gray-500 text-sm">
            <span class="font-bold">Company:</span> Tisalabs &nbsp;&nbsp; | &nbsp;&nbsp;
            <span class="font-bold">Technologies:</span> Vue.js, Firebase, Python Flask, Tailwind
          </p>
          <a href="#" class="text-blue-500 text-sm underline mt-2 inline-block">Check Project →</a>
        </div>
        <img
          src="../assets/images/TridentApp2.png"
          alt="TridentApp"
          class="rounded-lg shadow-lg w-full md:w-1/3"
        />
      </div>

      <!-- Third Project -->
      <div class="flex flex-col md:flex-row items-start md:items-center gap-6">
        <div class="flex-1">
          <h2 class="text-lg md:text-xl font-bold text-gray-800 mb-2">OFZONE Agency Website</h2>
          <p class="text-gray-600 text-sm md:text-base mb-4">
            Collaboration: Team of Software Engineers In partnership with a team
            of developers, I created a sleek, modern website for OFZONE Agency.
            Built with Next.js, the platform is optimized for fast loading
            times, SEO, and a smooth user experience. This project highlights my
            ability to work collaboratively and deliver exceptional results.
          </p>
          <p class="text-gray-500 text-sm">
            <span class="font-bold">Company:</span> OFZONE Agency &nbsp;&nbsp; | &nbsp;&nbsp;
            <span class="font-bold">Technologies:</span> Next.js, Tailwind
          </p>
          <a href="#" class="text-blue-500 text-sm underline mt-2 inline-block">Check Project →</a>
        </div>
        <img
          src="../assets/images/Offzoneagency.png"
          alt="OFZONE Agency Website"
          class="rounded-lg shadow-lg w-full md:w-1/3"
        />
      </div>
    </div>
  </section>
</template>

<style scoped>
/* Add any custom styles here if needed */
</style>

