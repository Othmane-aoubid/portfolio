<template>
  <nav class="fixed w-full bg-[#0D1117] z-50 px-6 py-4">
    <div class="max-w-7xl mx-auto flex justify-between items-center">
      <!-- Logo -->
      <div class="flex items-center">
        <span class="text-white ml-2 font-semibold">Othmane <span class="text-[#00FF95]">Aoubid</span></span>
      </div>

      <!-- Navigation Links -->
      <div class="hidden md:flex space-x-6">
        <router-link 
          v-for="item in navItems" 
          :key="item.path"
          :to="item.path"
          class="text-gray-300 hover:text-[#00FF95] transition-colors"
        >
          {{ item.name }}
        </router-link>
      </div>

      <!-- Mobile Menu Button -->
      <button @click="toggleMenu" class="md:hidden text-white">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
        </svg>
      </button>
    </div>

    <!-- Mobile Menu -->
    <div v-if="isMenuOpen" class="md:hidden absolute top-16 left-0 w-full bg-[#0D1117] py-4 px-6">
      <router-link 
        v-for="item in navItems" 
        :key="item.path"
        :to="item.path"
        class="block py-2 text-gray-300 hover:text-[#00FF95] transition-colors"
        @click="closeMenu"
      >
        {{ item.name }}
      </router-link>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavBar',
  data() {
    return {
      isMenuOpen: false,
      navItems: [
        { name: 'Home', path: '/' },
        { name: 'About', path: '/about' },
        { name: 'Projects', path: '/projects' },
        { name: 'Experience', path: '/experience' },
        { name: 'Certificates', path: '/certificates' },
        { name: 'Contact', path: '/contact' }
      ]
    }
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen
    },
    closeMenu() {
      this.isMenuOpen = false
    }
  }
}
</script>
