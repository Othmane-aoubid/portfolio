<template>
  <section class="py-20 px-6 bg-[#0D1117]" style="border-top: 3px solid">
    <div class="max-w-7xl mx-auto">
      <h2 class="text-3xl font-semibold text-center mb-16 text-white relative">
        About Me
        <div
          class="absolute bottom-0 left-1/2 transform -translate-x-1/2 w-16 h-1 bg-[#00FF95] mt-2"
        ></div>
      </h2>

      <div class="flex flex-col md:flex-row gap-12">
        <!-- Profile Image -->
        <div
          class="w-64 h-64 bg-gray-200 rounded-lg overflow-hidden flex-shrink-0"
        >
          <img
            src="../assets/images/othmaneaoubid.jpg"
            alt="Profile"
            class="w-full h-full object-cover"
          />
        </div>

        <!-- Profile Info -->
        <div class="flex-grow">
          <h3 class="text-2xl font-semibold mb-4 text-white">Othmane Aoubid</h3>
          <p class="text-gray-400 mb-8 max-w-2xl">
            I'm a dedicated developer with expertise in web development,
            networking, and AI technologies. With a strong foundation in both
            frontend and backend development, I create responsive and
            user-friendly applications.
          </p>

          <!-- Contact Info -->
          <div class="flex flex-col space-y-4">
            <div class="flex items-center gap-6">
              <!-- <div class="flex items-center gap-3">
                <div class="w-8 h-8 rounded-full bg-[#00FF95]/20 flex items-center justify-center">
                  <svg class="w-4 h-4 text-[#00FF95]" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M6.54 5C6.6 5.89 6.75 6.76 6.99 7.59L5.79 8.79C5.38 7.59 5.12 6.32 5.03 5H6.54M16.4 17.02C17.25 17.26 18.12 17.41 19 17.47V18.96C17.68 18.87 16.41 18.61 15.2 18.21L16.4 17.02M4.95 19H3C2.45 19 2 18.55 2 18V3C2 2.45 2.45 2 3 2H21C21.55 2 22 2.45 22 3V18C22 18.55 21.55 19 21 19H19.05L17 21.05L14.96 19H4.95Z"/>
                  </svg>
                </div>
                <span class="text-gray-400">+212 600 000 000</span>
              </div> -->
              <!-- <div class="flex items-center gap-3">
                <div class="w-8 h-8 rounded-full bg-[#00FF95]/20 flex items-center justify-center">
                  <svg class="w-4 h-4 text-[#00FF95]" fill="currentColor" viewBox="0 0 24 24">
                    <path d="M20 4H4C2.9 4 2 4.9 2 6V18C2 19.1 2.9 20 4 20H20C21.1 20 22 19.1 22 18V6C22 4.9 21.1 4 20 4ZM20 8L12 13L4 8V6L12 11L20 6V8Z"/>
                  </svg>
                </div>
                <span class="text-gray-400">othmaneaoubid11@gmail.com</span>
              </div> -->
            </div>
            <div class="flex items-center gap-6">
              <div class="flex items-center gap-3">
                <div
                  class="w-8 h-8 rounded-full bg-[#00FF95]/20 flex items-center justify-center"
                >
                  <svg
                    class="w-4 h-4 text-[#00FF95]"
                    fill="currentColor"
                    viewBox="0 0 24 24"
                  >
                    <path
                      d="M12 2C8.13 2 5 5.13 5 9C5 14.25 12 22 12 22C12 22 19 14.25 19 9C19 5.13 15.87 2 12 2ZM12 11.5C10.62 11.5 9.5 10.38 9.5 9C9.5 7.62 10.62 6.5 12 6.5C13.38 6.5 14.5 7.62 14.5 9C14.5 10.38 13.38 11.5 12 11.5Z"
                    />
                  </svg>
                </div>
                <span class="text-gray-400">Casablanca, Morocco</span>
              </div>
              <div class="flex items-center gap-3">
                <div
                  class="w-8 h-8 rounded-full bg-[#00FF95]/20 flex items-center justify-center"
                >
                  <svg
                    class="w-4 h-4 text-[#00FF95]"
                    fill="currentColor"
                    viewBox="0 0 24 24"
                  >
                    <path
                      d="M12 12C14.21 12 16 10.21 16 8C16 5.79 14.21 4 12 4C9.79 4 8 5.79 8 8C8 10.21 9.79 12 12 12ZM12 14C9.33 14 4 15.34 4 18V20H20V18C20 15.34 14.67 14 12 14Z"
                    />
                  </svg>
                </div>
                <span class="text-gray-400">Full Stack Developer</span>
              </div>
            </div>
          </div>

          <!-- Social Links -->
          <div class="flex gap-4 mt-8">
            <a
              href="https://www.linkedin.com/in/othmane-aoubid-397417147/"
              target="_blank"
              rel="noopener noreferrer"
              class="w-8 h-8 rounded-full bg-[#1A1F29] flex items-center justify-center"
            >
              <svg
                class="w-4 h-4 text-gray-400"
                fill="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"
                />
              </svg>
            </a>
            <a
              href="https://github.com/Othmane-aoubid?tab=repositories"
              target="_blank"
              rel="noopener noreferrer"
              class="w-8 h-8 rounded-full bg-[#1A1F29] flex items-center justify-center"
            >
              <svg
                class="w-4 h-4 text-gray-400"
                fill="currentColor"
                viewBox="0 0 24 24"
              >
                <path
                  d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"
                />
              </svg>
            </a>
          </div>
        </div>
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
