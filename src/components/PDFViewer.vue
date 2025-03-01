<template>
  <div class="pdf-container">
    <embed
      :src="pdfUrl"
      type="application/pdf"
      class="w-full h-full"
      width="100%"
      height="100%"
    />
  </div>
</template>

<script>
export default {
  name: 'PDFViewer',
  props: {
    pdfUrl: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
.pdf-container {
  width: 100%;
  height: 100vh;
  max-height: 800px;
  position: relative;
  border-radius: 0.5rem;
  background: white;
  overflow: hidden;
}

@media (max-width: 768px) {
  .pdf-container {
    height: 70vh;
  }
}
</style>
