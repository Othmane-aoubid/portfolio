<template>
  <section class="py-12">
    <div class="text-center mb-8">
      <h2 class="text-4xl font-bold text-gray-900">Client Feedback</h2>
      <p class="text-gray-600 mt-3">Here's what our clients say about Othmane's exceptional work.</p>
    </div>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 px-6">
      <div v-for="feedback in feedbacks" :key="feedback.id" class="bg-white p-6 rounded-lg shadow-lg">
        <div class="flex items-center mb-4">
          <div class="flex items-center">
            <span class="text-yellow-500">
              <i class="fas fa-star"></i>
              <i class="fas fa-star"></i>
              <i class="fas fa-star"></i>
              <i class="fas fa-star"></i>
              <i class="fas fa-star"></i>
            </span>
          </div>
        </div>
        <p class="text-gray-700 mb-4">{{ feedback.message }}</p>
        <div class="flex items-center">
          <img :src="feedback.image" alt="Client" class="w-10 h-10 rounded-full mr-3">
          <div>
            <h4 class="font-semibold">{{ feedback.name }}</h4>
            <p class="text-gray-500">{{ feedback.position }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      feedbacks: [
        {
          id: 1,
          message: "Othmane delivered our project ahead of schedule and exceeded our expectations with his innovative solutions.",
          name: "Sarah Johnson",
          position: "Project Manager at Tech Solutions",
        },
        {
          id: 2,
          message: "Working with Othmane was a game-changer for our web application. His expertise in both front-end and back-end development is impressive.",
          name: "Michael Smith",
          position: "CEO of Creative Agency",
        },
        {
          id: 3,
          message: "His coding skills are top-notch, and he always finds practical solutions to complex problems.",
          name: "David Brown",
          position: "Product Owner at StartUp Inc.",
        },
        {
          id: 4,
          message: "Othmane's work on our e-commerce platform was outstanding. He truly understands user experience.",
          name: "Laura Wilson",
          position: "Marketing Director at E-commerce Hub",
        },
        {
          id: 5,
          message: "A talented developer who is always eager to learn and improve. Othmane is a valuable asset to any team.",
          name: "James Taylor",
          position: "Technical Lead at Web Innovations",
        },
        {
          id: 6,
          message: "Othmane's attention to detail and ability to collaborate made our project a success. Highly recommend him!",
          name: "Emily Davis",
          position: "Lead Designer at Design Co.",
        },
      ],
    };
  },
};
</script>

<style scoped>
/* Add any additional styles here */
</style>
