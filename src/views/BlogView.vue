<template>
  <div class="max-w-7xl mx-auto p-6 py-20">
    <!-- Header Section -->
    <h1 class="text-2xl md:text-4xl font-bold text-gray-800 mb-4 text-center">Othmane's Insights</h1>
    <p class="text-lg text-center text-gray-600 mb-8">
      Dive into the world of web development with articles that share practical
      tips, personal experiences, and the latest trends in technology.
    </p>

    <!-- Recent Articles Section -->
    <section class="mb-12">
      <div class="flex justify-between items-center mb-6">
        <h2 class="text-1xl md:text-2xl font-bold text-gray-800 mb-4">Recent Articles</h2>
        <a href="#" class="text-blue-600 hover:underline text-sm font-medium"
          >View All</a
        >
      </div>
      <div class="grid md:grid-cols-4 gap-6">
        <div
          v-for="article in recentArticles"
          :key="article.title"
          class="bg-white shadow-md rounded-lg overflow-hidden"
        >
          <img
            :src="article.image"
            :alt="article.title"
            class="w-full h-40 object-cover"
          />
          <div class="p-4">
            <h3 class="text-1xl md:text-2xl font-bold text-gray-800 mb-4">{{ article.title }}</h3>
            <p class="text-sm text-gray-600">{{ article.category }}</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Additional Resources Section -->
    <section>
      <h2 class="text-2xl md:text-4xl font-bold text-gray-800 mb-4 text-center">Additional Resources</h2>
      <div class="grid md:grid-cols-4 gap-6">
        <div
          v-for="resource in additionalResources"
          :key="resource.title"
          class="bg-white shadow-md rounded-lg overflow-hidden"
        >
          <img
            :src="resource.image"
            :alt="resource.title"
            class="w-full h-40 object-cover"
          />
          <div class="p-4">
            <h3 class="text-1xl md:text-2xl font-bold text-gray-800 mb-4">{{ resource.title }}</h3>
            <p class="text-sm text-gray-600">{{ resource.category }}</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      recentArticles: [
        {
          title: "The Journey of a Full Stack Developer",
          category: "Front-End Development",
          image: "https://via.placeholder.com/300x200",
        },
        {
          title: "Top JavaScript Frameworks for 2023",
          category: "Web Development",
          image: "https://via.placeholder.com/300x200",
        },
        {
          title: "Best Practices for Optimizing Web Applications",
          category: "Web Performance",
          image: "https://via.placeholder.com/300x200",
        },
        {
          title: "The Importance of Collaboration in Development",
          category: "Teamwork",
          image: "https://via.placeholder.com/300x200",
        },
      ],
      additionalResources: [
        {
          title: "The Journey of a Full Stack Developer",
          category: "Front-End Development",
          image: "https://via.placeholder.com/300x200",
        },
        {
          title: "Top JavaScript Frameworks for 2023",
          category: "Web Development",
          image: "https://via.placeholder.com/300x200",
        },
        {
          title: "Best Practices for Optimizing Web Applications",
          category: "Web Performance",
          image: "https://via.placeholder.com/300x200",
        },
        {
          title: "The Importance of Collaboration in Development",
          category: "Teamwork",
          image: "https://via.placeholder.com/300x200",
        },
      ],
    };
  },
};
</script>

<style>
/* Add additional custom styles if necessary */
</style>
