<template>
  <div class="max-w-4xl mx-auto p-6 py-20">
    <h2 class="text-2xl md:text-4xl font-bold text-gray-800 mb-4 text-center">
      Professional Journey
    </h2>
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
          <h4
            class="text-lg font-bold text-black-600"
            style="color: #4d97e3 !important"
          >
            {{ experience.title }}
          </h4>
          <button>
            <span
              v-if="expandedIndex === index"
              class="text-xl font-bold text-black-600"
              style="color: #4d97e3 !important"
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
          <ul class="list-disc pl-5 space-y-2">
            <li
              v-for="(item, itemIndex) in experience.description"
              :key="itemIndex"
            >
              {{ item }}
            </li>
          </ul>
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
          title:
            "Full Stack Developer at Tisalabs (February 2023 - August 2024) - Morocco, Casablanca",
          description: [
            "Designed and implemented front-end features for Predictive, asecurity threat scanning platform, using Vue.js for a seamless userinterface.",
            "Developed back-end APIs with Python Flask to process real-timedata and predict vulnerabilities using advanced algorithms.",
            "Integrated Firebase for secure authentication and database management.",
            "Enhanced application performance by implementing optimization techniques, reducing scan time by 20%.",
            "Built and optimized the e-commerce platform",
            "Ensured seamless user experience",
            "Implemented robust back-end functionality",
            "Collaborated with cross-functional teams",
            "Conducted rigorous testing and debugging to ensure high reliability and scalability of the platform",
            "Collaborated with security experts to align application functionality with industry standards",
            "Designed and deployed Trident, an energy monitoring application in partnership with the Irish government",
            "Built back-end infrastructure with Python Flask for tracking and managing energy transactions",
            "Implemented real-time energy data visualizations and dashboards using Vue.js",
            "Worked closely with government representatives and stakeholders to meet project specifications and deadlines"
          ],
        },
        {
          title:
            "Front-end Developer at Offzone Agency (April 2022 - July 2023) - Morocco, Casablanca",
            description: [
            "Worked on various freelance projects",
            "Delivered custom web solutions for clients",
            "Focused on performance and scalability",
            "Utilized modern front-end technologies",
            "Developed Offzone Agency's official website using Next.js, ensuring optimal performance and responsiveness",
            "Integrated SEO techniques to improve search engine visibility and user engagement",
            "Collaborated with the development team to create user-friendly navigation and intuitive interfaces",
            "Implemented Google Analytics to monitor and report on website traffic and user behavior",
            "Ensured mobile responsiveness and cross-browser compatibility of all website components",
            "Participated in design and UI/UX discussions, contributing to an enhanced user experience",
            "Utilized styled components and Tailwind CSS for efficient styling and faster development",
            "Monitored and optimized website loading speed through effective asset management",
            "Conducted regular code reviews and implemented improvements based on feedback",
            "Provided support for maintaining and updating the website post-launch"
          ],
        },
        {
          title:
            "Front-end Developer at Clicknetkey (January 2022 - March 2022) - Morocco, Casablanca",
            description: [
            "Supported the development of internal applications",
            "Collaborated with the team to deliver efficient solutions",
            "Implemented responsive designs",
            "Contributed to code reviews and documentation",
            "Designed and built a React.js-based application to monitor and register soccer game data",
            "Created interactive components to record player statistics and game events in real time",
            "Ensured state management using Redux for seamless data flow across the application",
            "Conducted front-end testing to identify and resolve bugs and usability issues",
            "Collaborated with team members to refine the application's functionality and design",
            "Improved application performance through effective use of React lifecycle methods",
            "Developed reusable components for consistent design and improved efficiency",
            "Integrated APIs for fetching and displaying match-related data dynamically",
            "Created responsive layouts compatible with various screen sizes and devices",
            "Documented the application's features and functionality for future maintenance"
          ],
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
