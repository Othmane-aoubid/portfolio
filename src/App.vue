<template>
  <div class="min-h-screen bg-[#0D1117]">
    <NavBar />
    <router-view />
    <Footer/>
  </div>
</template>

<script>
import NavBar from '@/components/NavBar.vue'
import Footer from './components/footer/Footer.vue';
export default {
  name: 'App',
  components: {
    NavBar,
    Footer
  }
}
</script>

<style>
@import './assets/main.css';

body {
  margin: 0;
  padding: 0;
  font-family: 'Inter', sans-serif;
  background-color: #0D1117;
  color: white;
}

::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: #0D1117;
}

::-webkit-scrollbar-thumb {
  background: #00FF95;
  border-radius: 4px;
}

::-webkit-scrollbar-thumb:hover {
  background: #00cc78;
}
</style>
