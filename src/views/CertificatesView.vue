<template>
  <div class="min-h-screen bg-gradient-to-br from-gray-900 via-gray-800 to-gray-900 py-16">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Header -->
      <div class="text-center mb-16">
        <h2 class="text-4xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-blue-400 to-emerald-400 sm:text-5xl">
          Professional Certifications
        </h2>
        <div class="mt-4 text-xl text-gray-400 max-w-2xl mx-auto">
          Showcasing my continuous learning journey and professional development
        </div>
      </div>

      <!-- Certificate Categories -->
      <div class="space-y-24">
        <CertificateSection
          title="IT & Networking"
          subtitle="Cisco Networking Academy Certifications"
          :certificates="networkingCerts"
          gradient-colors="from-blue-500 to-blue-600"
          hover-color="blue-400"
        >
          <template #icon>
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4m6 6v10m6-2a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4" />
            </svg>
          </template>
        </CertificateSection>

        <CertificateSection
          title="Programming & Linux"
          subtitle="System Administration & Development"
          :certificates="programmingCerts"
          gradient-colors="from-purple-500 to-purple-600"
          hover-color="purple-400"
        >
          <template #icon>
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 9l3 3-3 3m5 0h3M5 20h14a2 2 0 002-2V6a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" />
            </svg>
          </template>
        </CertificateSection>

        <CertificateSection
          title="AI & Machine Learning"
          subtitle="Advanced AI and Neural Networks"
          :certificates="aiCerts"
          gradient-colors="from-emerald-500 to-emerald-600"
          hover-color="emerald-400"
        >
          <template #icon>
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9 20l-1 1h8l-1-1-.75-3M3 13h18M5 17h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
            </svg>
          </template>
        </CertificateSection>
      </div>
    </div>
  </div>
</template>

<script>
import CertificateSection from '../components/CertificateSection.vue'

export default {
  name: 'CertificatesView',
  components: {
    CertificateSection
  },
  data() {
    return {
      networkingCerts: [
        {
          title: 'AWS Academy Cloud Foundations',
          issuer: 'AWS Academy',
          date: '2024',
          image: '/certificates/aws-academy-graduate-aws-academy-cloud-foundations.png'
        },
        {
          title: 'Networking Essentials',
          issuer: 'Cisco Networking Academy',
          date: '2023',
          image: '/certificates/Networking_Essentials_certificate_o_aoubid-etu-enset-media-ac-ma_63d735e0-2607-4452-8c2b-002c29508430_page-0001.jpg'
        },
        {
          title: 'English for IT 1',
          issuer: 'Cisco Networking Academy',
          date: '2023',
          image: '/certificates/English_for_IT_1_certificate_o_aoubid-etu-enset-media-ac-ma_36946776-5e5f-4131-a695-3f7b895b7656_page-0001.jpg'
        },
        {
          title: 'Introduction to IoT',
          issuer: 'Cisco Networking Academy',
          date: '2023',
          image: '/certificates/Introduction_to_IoT_certificate_o_aoubid-etu-enset-media-ac-ma_e272b145-044d-48d8-8aee-c27ba8e801a7_page-0001.jpg'
        },
        {
          title: 'Principles of Cybersecurity',
          issuer: 'Cisco Networking Academy',
          date: '2023',
          image: '/certificates/_certificate_o_aoubid-Principles-of- Cybersecurity_page-0001.jpg'
        }
      ],
      programmingCerts: [
        {
          title: 'NDG Linux Unhatched',
          issuer: 'NDG Linux',
          date: '2023',
          image: '/certificates/Partner-_NDG_Linux_Unhatched_certificate_o_aoubid-etu-enset-media-ac-ma_b77d576a-16fa-4297-ab42-b77633b5036c_page-0001.jpg'
        },
        {
          title: 'Linux Essentials',
          issuer: 'Linux Professional Institute',
          date: '2023',
          image: '/certificates/aoubidothmane-certificate-LINUX ESSENTIALS_page-0001.jpg'
        }
      ],
      aiCerts: [
        {
          title: 'Intro to ChatGPT and Generative AI',
          issuer: 'Coursera',
          date: '2023',
          image: '/certificates/othamen-Intro to ChatGPT and Generative AI_page-0001.jpg'
        },
        {
          title: 'Build Chat Applications with OpenAI',
          issuer: 'Coursera',
          date: '2023',
          image: '/certificates/othmane-Build Chat Applications with OpenAI_page-0001.jpg'
        },
        {
          title: 'Convolutional Neural Networks',
          issuer: 'Coursera',
          date: '2023',
          image: '/certificates/othmane-Convolutional Neural Networks with_page-0001.jpg'
        }
      ]
    }
  }
}
</script>
