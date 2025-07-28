<template>
  <div class="min-h-screen bg-gray-50">
    <!-- Social Media Icons - Sticky -->
    <LandingSocialMedia />

    <!-- Main Content -->
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 py-16">

      <!-- Page Header -->
      <section class="text-center mb-16 pt-8 lg:pt-16">
        <h1 class="text-4xl sm:text-5xl lg:text-6xl font-bold text-gray-900 mb-6 font-barlow-condensed">
          Get In <span class="text-blue-600">Touch</span>
        </h1>
        <div class="w-24 h-1 bg-blue-600 rounded-full mx-auto mb-8"></div>
        <p class="text-lg text-gray-700 max-w-2xl mx-auto leading-relaxed">
          Ready to transform your business? Let's discuss how we can help you achieve your goals.
        </p>
      </section>

      <!-- Contact Information -->
      <section class="mb-16">
        <div class="grid md:grid-cols-2 gap-12 max-w-4xl mx-auto">

          <!-- Contact Details -->
          <div class="bg-white rounded-2xl shadow-lg p-8">
            <h2 class="text-2xl font-bold text-gray-900 mb-8 font-barlow-condensed text-center">
              Contact Information
            </h2>

            <!-- Phone -->
            <div class="flex items-start gap-4 mb-8">
              <div class="w-16 h-16 flex-shrink-0">
                <div ref="phoneAnimation" class="w-full h-full"></div>
              </div>
              <div>
                <h3 class="font-semibold text-gray-900 mb-2">Phone</h3>
                <p class="text-gray-700">+234 813 292 4637</p>
                <p class="text-gray-700">+234 813 292 4637</p>
              </div>
            </div>

            <!-- Email -->
            <div class="flex items-start gap-4 mb-8">
              <div class="w-16 h-16 flex-shrink-0 bg-blue-100 rounded-full flex items-center justify-center">
                <Icon name="heroicons:envelope" class="w-8 h-8 text-blue-600" />
              </div>
              <div>
                <h3 class="font-semibold text-gray-900 mb-2">Email</h3>
                <p class="text-gray-700">info@wilsonsamson.com</p>
              </div>
            </div>

            <!-- Location -->
            <div class="flex items-start gap-4">
              <div class="w-16 h-16 flex-shrink-0">
                <div ref="locationAnimation" class="w-full h-full"></div>
              </div>
              <div>
                <h3 class="font-semibold text-gray-900 mb-2">Location</h3>
                <p class="text-gray-700 leading-relaxed">
                  11 Adeshina Street, Off Olowu Street,<br>
                  Off Obafemi Awolowo Way,<br>
                  Ikeja, Lagos
                </p>
              </div>
            </div>
          </div>

          <!-- Contact Form -->
          <div class="bg-white rounded-2xl shadow-lg p-8">
            <h2 class="text-2xl font-bold text-gray-900 mb-8 font-barlow-condensed text-center">
              Send Us a Message
            </h2>

            <form @submit.prevent="submitForm" class="space-y-6">
              <div>
                <label for="name" class="block text-sm font-medium text-gray-700 mb-2">Full Name</label>
                <input type="text" id="name" v-model="form.name" required
                  class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-600 focus:border-transparent transition-all duration-300">
              </div>

              <div>
                <label for="email" class="block text-sm font-medium text-gray-700 mb-2">Email Address</label>
                <input type="email" id="email" v-model="form.email" required
                  class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-600 focus:border-transparent transition-all duration-300">
              </div>

              <div>
                <label for="phone" class="block text-sm font-medium text-gray-700 mb-2">Phone Number</label>
                <input type="tel" id="phone" v-model="form.phone"
                  class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-600 focus:border-transparent transition-all duration-300">
              </div>

              <div>
                <label for="subject" class="block text-sm font-medium text-gray-700 mb-2">Subject</label>
                <input type="text" id="subject" v-model="form.subject" required
                  class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-600 focus:border-transparent transition-all duration-300">
              </div>

              <div>
                <label for="message" class="block text-sm font-medium text-gray-700 mb-2">Message</label>
                <textarea id="message" v-model="form.message" rows="4" required
                  class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-600 focus:border-transparent transition-all duration-300 resize-vertical"></textarea>
              </div>

              <button type="submit" :disabled="isSubmitting"
                class="w-full bg-blue-600 hover:bg-blue-700 disabled:bg-blue-400 text-white font-semibold py-3 px-6 rounded-lg transition-colors duration-300 font-barlow-condensed text-lg tracking-wide">
                {{ isSubmitting ? 'SENDING...' : 'SEND MESSAGE' }}
              </button>
            </form>
          </div>
        </div>
      </section>

      <!-- Quick Contact CTA -->
      <section class="text-center">
        <div class="bg-gray-900 rounded-2xl p-8 text-white max-w-2xl mx-auto">
          <h3 class="text-2xl font-bold mb-4 font-barlow-condensed">
            Need Immediate Assistance?
          </h3>
          <p class="text-gray-300 mb-6">
            For urgent inquiries, reach out to us directly via WhatsApp
          </p>
          <a href="https://wa.me/2348132924637" target="_blank" rel="noopener noreferrer"
            class="inline-flex items-center gap-3 bg-green-600 hover:bg-green-700 text-white px-6 py-3 rounded-lg font-semibold transition-colors duration-300">
            <Icon name="logos:whatsapp-icon" class="w-5 h-5" />
            Chat on WhatsApp
          </a>
        </div>
      </section>
    </div>
  </div>
</template>

<script setup>
// Define page layout
definePageMeta({
  layout: "landing"
})

// SEO meta
useHead({
  title: 'Contact Us - Wilson Samson | Leadership & Business Excellence',
  meta: [
    {
      name: 'description',
      content: 'Get in touch with Wilson Samson for leadership consulting, employee engagement, and organizational excellence services. Contact us today!'
    }
  ]
})

// Form state
const form = ref({
  name: '',
  email: '',
  phone: '',
  subject: '',
  message: ''
})

const isSubmitting = ref(false)

// Template refs for Lottie animations
const phoneAnimation = ref(null)
const locationAnimation = ref(null)

// Form submission handler
const submitForm = async () => {
  isSubmitting.value = true

  try {
    // Here you would typically send the form data to your backend
    // For now, we'll just simulate a successful submission
    await new Promise(resolve => setTimeout(resolve, 1000))

    // Show success message
    alert('Thank you for your message! We will get back to you soon.')

    // Reset form
    form.value = {
      name: '',
      email: '',
      phone: '',
      subject: '',
      message: ''
    }
  } catch (error) {
    alert('Sorry, there was an error sending your message. Please try again.')
  } finally {
    isSubmitting.value = false
  }
}

// Initialize Lottie animations on mount
onMounted(async () => {
  try {
    // Dynamically import lottie-web
    const lottie = await import('lottie-web')

    // Phone animation
    if (phoneAnimation.value) {
      lottie.default.loadAnimation({
        container: phoneAnimation.value,
        renderer: 'svg',
        loop: true,
        autoplay: true,
        path: 'https://lottie.host/3ee84bbb-612e-4ebb-b558-0d0617467073/9VSKxPEINM.lottie'
      })
    }

    // Location animation
    if (locationAnimation.value) {
      lottie.default.loadAnimation({
        container: locationAnimation.value,
        renderer: 'svg',
        loop: true,
        autoplay: true,
        path: 'https://lottie.host/fadaf240-98c6-42fe-a1b2-56777059f554/51q7mWaDJN.lottie'
      })
    }
  } catch (error) {
    console.error('Error loading Lottie animations:', error)
  }
})
</script>

<style scoped>
/* Custom transitions for form elements */
input:focus,
textarea:focus {
  outline: none;
}

/* Smooth transitions */
* {
  transition-property: color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, backdrop-filter;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 150ms;
}

/* Focus styles */
input:focus,
textarea:focus,
button:focus {
  outline: 2px solid #3B82F6;
  outline-offset: 2px;
}
</style>