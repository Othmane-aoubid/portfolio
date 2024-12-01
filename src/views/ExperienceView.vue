<template>
  <div class="max-w-4xl mx-auto p-6 py-20">
    <h2 class="text-2xl md:text-4xl font-bold text-gray-800 mb-4 text-center">Professional Journey</h2>
    <p class="text-lg text-center text-gray-600 mb-8">
      With over two years of experience, Othmane has successfully built and
      optimized web applications, showcasing his expertise in both front-end and
      back-end development.
    </p>

    <h3 class="text-2xl font-bold text-center mb-6">Experience Timeline</h3>
    <div>
      <div
        v-for="(experience, index) in experiences"
        :key="index"
        class="border-b border-gray-300 mb-4"
      >
        <div
          class="flex justify-between items-center p-4 cursor-pointer hover:bg-gray-50"
          @click="toggleExperience(index)"
        >
          <h4 class="text-lg font-bold text-black-600" style="color: #4D97E3 !important;">{{ experience.title }}</h4>
          <button>
            <span
              v-if="expandedIndex === index"
              class="text-xl font-bold text-black-600"
              style="color: #4D97E3 !important;"
            >
              -
            </span>
            <span v-else class="text-xl font-bold text-gray-600"> + </span>
          </button>
        </div>
        <div
          v-if="expandedIndex === index"
          class="p-4 text-gray-700 bg-gray-100"
        >
          <p>{{ experience.description }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      expandedIndex: null,
      experiences: [
        {
          title: "Full Stack Developer at Online Retailer (2023-05)",
          description:
            "As a Full Stack Developer, I was responsible for building and optimizing the e-commerce platform, ensuring a seamless user experience and robust back-end functionality.",
        },
        {
          title: "Web Developer at Freelance (2023-01)",
          description:
            "Worked on various freelance projects, delivering custom web solutions for clients, focusing on performance and scalability.",
        },
        {
          title: "Junior Developer at Tech Solutions (2022-11)",
          description:
            "Supported the development of internal applications, collaborating with the team to deliver efficient and effective solutions.",
        },
      ],
    };
  },
  methods: {
    toggleExperience(index) {
      this.expandedIndex = this.expandedIndex === index ? null : index;
    },
  },
};
</script>

<style>
/* Add any additional styling if needed */
</style>
