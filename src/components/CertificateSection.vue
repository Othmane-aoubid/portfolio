<template>
  <section>
    <div class="flex items-center mb-8">
      <div class="flex-shrink-0">
        <div :class="`h-12 w-12 rounded-xl bg-gradient-to-br ${gradientColors} flex items-center justify-center shadow-lg`">
          <slot name="icon"></slot>
        </div>
      </div>
      <div class="ml-6">
        <h3 class="text-2xl font-bold text-white">{{ title }}</h3>
        <p class="text-gray-400 mt-1">{{ subtitle }}</p>
      </div>
    </div>
    
    <div class="grid gap-8 md:grid-cols-1 lg:grid-cols-1">
      <div v-for="cert in certificates" :key="cert.title" 
           :class="`group relative bg-gray-800/50 backdrop-blur rounded-2xl overflow-hidden transition-all duration-300 hover:shadow-xl hover:shadow-${hoverColor}/10`">
        <div :class="`absolute inset-0 bg-gradient-to-br ${gradientColors}/10 opacity-0 group-hover:opacity-100 transition-opacity`"></div>
        <div class="relative">
          <div class="flex items-center justify-between p-6 border-b border-gray-700">
            <div>
              <h4 :class="`text-xl font-semibold text-white group-hover:text-${hoverColor} transition-colors`">{{ cert.title }}</h4>
              <p class="text-gray-400 mt-1">{{ cert.issuer }}</p>
            </div>
            <span class="text-sm text-gray-500 bg-gray-800/50 px-3 py-1 rounded-full">{{ cert.date }}</span>
          </div>
          <div class="p-1 bg-white">
            <PDFViewer :pdf-url="cert.image" />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import PDFViewer from './PDFViewer.vue'

export default {
  name: 'CertificateSection',
  components: {
    PDFViewer
  },
  props: {
    title: {
      type: String,
      required: true
    },
    subtitle: {
      type: String,
      required: true
    },
    certificates: {
      type: Array,
      required: true
    },
    gradientColors: {
      type: String,
      required: true
    },
    hoverColor: {
      type: String,
      required: true
    }
  }
}
</script>
