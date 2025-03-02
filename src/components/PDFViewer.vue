<template>
  <div class="pdf-container">
    <embed
      :src="pdfUrl"
      type="application/pdf"
      class="pdf-embed"
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
  height: 500px; /* Default height for larger screens */
  border-radius: 0.5rem;
  overflow: hidden;
}

.pdf-embed {
  width: 100%;
  height: 100%;
}

/* Media query for smaller screens */
@media (max-width: 768px) {
  .pdf-container {
    height: auto;     /* Allow container to shrink or expand based on content */
    min-height: 300px; /* Optional: ensure it doesn't get too small */
  }

  .pdf-embed {
    height: 100%;
    min-height: 300px; /* Same optional minimum to maintain visibility */
  }
}
</style>
