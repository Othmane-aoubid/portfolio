<template>
  <div class="bg-[#0D1117] px-6 py-24 sm:py-32 lg:px-8">
    <div class="mx-auto max-w-7xl">
      <h2 class="text-4xl font-semibold text-center mb-16 text-white">Get In Touch</h2>
      
      <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
        <!-- Contact Information -->
        <div class="text-white">
          <h3 class="text-2xl font-semibold mb-8">Contact Information</h3>
          
          <div class="space-y-6">
            <!-- <div class="flex items-center gap-4">
              <div class="w-10 h-10 bg-[#00FF95]/10 rounded-full flex items-center justify-center">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-[#00FF95]" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
                </svg>
              </div>
              <div>
                <p class="text-gray-400">Phone</p>
                <p>+212 600 000 000</p>
              </div>
            </div> -->

            <div class="flex items-center gap-4">
              <div class="w-10 h-10 bg-[#00FF95]/10 rounded-full flex items-center justify-center">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-[#00FF95]" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                </svg>
              </div>
              <div>
                <p class="text-gray-400">Email</p>
                <p>othmaneaoubid11@gmail.com</p>
              </div>
            </div>

            <div class="flex items-center gap-4">
              <div class="w-10 h-10 bg-[#00FF95]/10 rounded-full flex items-center justify-center">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-[#00FF95]" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
                </svg>
              </div>
              <div>
                <p class="text-gray-400">Location</p>
                <p>Casablanca, Morocco</p>
              </div>
            </div>
          </div>
        </div>

        <!-- Contact Form -->
        <div>
          <h3 class="text-2xl font-semibold mb-8 text-white">Send a Message</h3>
          <form @submit.prevent="submitForm" class="space-y-6">
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
              <div>
                <input
                  v-model="formData.firstName"
                  type="text"
                  name="first-name"
                  id="first-name"
                  placeholder="Name"
                  autocomplete="given-name"
                  class="block w-full rounded-lg bg-[#1A1F29] px-4 py-3 text-white border border-gray-700 focus:border-[#00FF95] focus:outline-none"
                  required
                />
              </div>
              <div>
                <input
                  v-model="formData.email"
                  type="email"
                  name="email"
                  id="email"
                  placeholder="Email"
                  autocomplete="email"
                  class="block w-full rounded-lg bg-[#1A1F29] px-4 py-3 text-white border border-gray-700 focus:border-[#00FF95] focus:outline-none"
                  required
                />
              </div>
            </div>

            <div>
              <input
                v-model="formData.subject"
                type="text"
                name="subject"
                id="subject"
                placeholder="Subject"
                class="block w-full rounded-lg bg-[#1A1F29] px-4 py-3 text-white border border-gray-700 focus:border-[#00FF95] focus:outline-none"
                required
              />
            </div>

            <div>
              <textarea
                v-model="formData.message"
                name="message"
                id="message"
                rows="4"
                placeholder="Message"
                class="block w-full rounded-lg bg-[#1A1F29] px-4 py-3 text-white border border-gray-700 focus:border-[#00FF95] focus:outline-none resize-none"
                required
              ></textarea>
            </div>

            <div>
              <button
                type="submit"
                :disabled="isSubmitting"
                class="w-full rounded-lg bg-[#00FF95] px-4 py-3 text-black font-semibold hover:bg-[#00FF95]/90 focus:outline-none disabled:opacity-50 disabled:cursor-not-allowed"
              >
                {{ isSubmitting ? "Sending..." : "Send Message" }}
              </button>
            </div>
          </form>

          <div
            v-if="submitStatus"
            :class="[
              'mt-4 p-4 rounded-lg',
              submitStatus.type === 'success'
                ? 'bg-green-100 text-green-700'
                : 'bg-red-100 text-red-700',
            ]"
          >
            {{ submitStatus.message }}
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, reactive, onMounted } from "vue";
import emailjs from "@emailjs/browser";

const formData = reactive({
  firstName: "",
  lastName: "",
  email: "",
  phoneNumber: "",
  subject: "",
  message: "",
});

const isSubmitting = ref(false);
const submitStatus = ref(null);

onMounted(() => {
  emailjs.init("fAQoijqTk9VVOKPhg");
});

const submitForm = async () => {
  isSubmitting.value = true;
  submitStatus.value = null;

  try {
    const templateParams = {
      to_email: "othmaneaoubid11@gmail.com",
      lastName: formData.lastName,
      firstName: formData.firstName,
      email: formData.email,
      phoneNumber: formData.phoneNumber,
      subject: formData.subject,
      message: formData.message,
    };

    await emailjs.send(
      "service_mn8wiji",
      "template_0is8ayj",
      templateParams
    );

    submitStatus.value = {
      type: "success",
      message: "Your message has been sent successfully!",
    };

    // Reset form
    Object.keys(formData).forEach((key) => (formData[key] = ""));
  } catch (error) {
    console.error("Error sending email:", error);
    submitStatus.value = {
      type: "error",
      message: "Failed to send message. Please try again later.",
    };
  } finally {
    isSubmitting.value = false;
  }
};
</script>
