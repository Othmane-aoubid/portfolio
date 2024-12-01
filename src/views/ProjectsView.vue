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
          <h2 class="text-lg md:text-xl font-bold text-gray-800 mb-2">E-commerce Platform</h2>
          <p class="text-gray-600 text-sm md:text-base mb-4">
            A fully functional e-commerce site showcasing products, allowing users to browse, purchase, and manage orders seamlessly.
          </p>
          <p class="text-gray-500 text-sm">
            <span class="font-bold">Date:</span> October 2023 &nbsp;&nbsp; | &nbsp;&nbsp;
            <span class="font-bold">Technologies:</span> HTML, CSS, JavaScript
          </p>
          <a href="#" class="text-blue-500 text-sm underline mt-2 inline-block">Check Project →</a>
        </div>
        <img
          src="https://via.placeholder.com/300x200"
          alt="E-commerce Platform"
          class="rounded-lg shadow-lg w-full md:w-1/3"
        />
      </div>

      <!-- Second Project -->
      <div class="flex flex-col md:flex-row items-start md:items-center gap-6 border-b pb-10">
        <div class="flex-1">
          <h2 class="text-lg md:text-xl font-bold text-gray-800 mb-2">Personal Blog</h2>
          <p class="text-gray-600 text-sm md:text-base mb-4">
            A blogging platform for sharing ideas and thoughts. Features include user authentication, posting, and commenting.
          </p>
          <p class="text-gray-500 text-sm">
            <span class="font-bold">Date:</span> January 2023 &nbsp;&nbsp; | &nbsp;&nbsp;
            <span class="font-bold">Technologies:</span> HTML, CSS, Tailwind
          </p>
          <a href="#" class="text-blue-500 text-sm underline mt-2 inline-block">Check Project →</a>
        </div>
        <img
          src="https://via.placeholder.com/300x200"
          alt="Personal Blog"
          class="rounded-lg shadow-lg w-full md:w-1/3"
        />
      </div>

      <!-- Third Project -->
      <div class="flex flex-col md:flex-row items-start md:items-center gap-6">
        <div class="flex-1">
          <h2 class="text-lg md:text-xl font-bold text-gray-800 mb-2">Portfolio Website</h2>
          <p class="text-gray-600 text-sm md:text-base mb-4">
            A personal portfolio showcasing my projects, experiences, and skills in web development and design.
          </p>
          <p class="text-gray-500 text-sm">
            <span class="font-bold">Date:</span> November 2022 &nbsp;&nbsp; | &nbsp;&nbsp;
            <span class="font-bold">Technologies:</span> HTML, CSS, JavaScript
          </p>
          <a href="#" class="text-blue-500 text-sm underline mt-2 inline-block">Check Project →</a>
        </div>
        <img
          src="https://via.placeholder.com/300x200"
          alt="Portfolio Website"
          class="rounded-lg shadow-lg w-full md:w-1/3"
        />
      </div>
    </div>
  </section>
</template>

<style scoped>
/* Add any custom styles here if needed */
</style>

