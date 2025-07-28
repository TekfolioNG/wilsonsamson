<template>
  <div class="min-h-screen bg-gray-50">
    <LandingSocialMedia />

    <!-- Hero Section - Added pt-24 to shift text down -->
    <section class=" bg-gray-900 py-12 sm:py-16 lg:pt-40 lg:pb-2">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
          <h1 class="text-3xl sm:text-4xl lg:text-5xl xl:text-6xl font-bold text-gray-200">
            Contact Us
          </h1>
          <p class="mt-4 sm:mt-6 text-lg sm:text-xl lg:text-2xl text-gray-400 max-w-3xl mx-auto leading-relaxed">
            We'd love to hear from you. Get in touch with us today.
          </p>
        </div>
      </div>
    </section>

    <!-- Our Address Section-->
    <section class="py-8 sm:py-10 lg:py-12 bg-gray-900">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="bg-gray-800 rounded-xl shadow-lg overflow-hidden">
          <div class="grid grid-cols-1 lg:grid-cols-2">
            <!-- Location Details Column -->
            <div
              class="p-4 sm:p-6 lg:p-8 flex flex-col justify-center items-center lg:items-start text-center lg:text-left order-2 lg:order-1">
              <h2 class="text-2xl sm:text-3xl lg:text-4xl font-bold text-gray-200 mb-4">Our Address</h2>

              <div class="flex items-start">
                <svg class="w-6 h-6 sm:w-7 sm:h-7 text-blue-400 mt-1 mr-4 flex-shrink-0" fill="none"
                  stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"></path>
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path>
                </svg>
                <div>
                  <p class="font-semibold text-gray-200 text-lg sm:text-xl mb-2">Address</p>
                  <p class="text-gray-300 leading-relaxed text-base sm:text-lg">
                    11 Adeshina Street, Off Olowu Street,<br>
                    Off Obafemi Awolowo Way,<br>
                    Ikeja, Lagos
                  </p>
                </div>
              </div>
            </div>
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-6 lg:gap-40">
              <!-- Lottie Animation Column -->
              <div class="p-4 sm:p-6 lg:p-8 flex items-center justify-center order-1 lg:order-2">
                <div class="w-full max-w-md">
                  <DotLottieVue style="height: 350px; width: 350px" autoplay loop
                    src="https://lottie.host/fadaf240-98c6-42fe-a1b2-56777059f554/51q7mWaDJN.lottie" />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact Details Section - Added dark bg -->
    <section class="py-8 sm:py-10 lg:py-8 bg-gray-900">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="bg-gray-800 rounded-xl shadow-lg overflow-hidden">
          <div class="grid grid-cols-1 lg:grid-cols-2 gap-6 lg:gap-40">
            <!-- Lottie Animation Column -->
            <div class="p-3 sm:p-4 lg:p-3 flex items-center justify-center">
              <div class="w-full max-w-md">
                <DotLottieVue style="height: 400px; width: 400px" autoplay loop
                  src="https://lottie.host/3ee84bbb-612e-4ebb-b558-0d0617467073/9VSKxPEINM.lottie" />
              </div>
            </div>

            <!-- Contact Details Column -->
            <div
              class="p-3 sm:p-4 lg:p-3 flex flex-col justify-center items-center lg:items-start text-center lg:text-left">
              <h2 class="text-2xl sm:text-3xl lg:text-4xl font-bold text-gray-200 mb-4">Get in Touch</h2>

              <div class="space-y-6 lg:space-y-8">
                <div class="flex items-start">
                  <svg class="w-6 h-6 sm:w-7 sm:h-7 text-blue-600 mt-1 mr-4 flex-shrink-0" fill="none"
                    stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z">
                    </path>
                  </svg>
                  <div>
                    <p class="font-semibold text-gray-200 text-lg sm:text-xl mb-1">Email</p>
                    <a href="mailto:info@wilsonsamson.com" class="text-blue-300 text-base sm:text-lg">
                      info@wilsonsamson.com
                    </a>
                  </div>
                </div>

                <div class="flex items-start">
                  <svg class="w-6 h-6 sm:w-7 sm:h-7 text-blue-600 mt-1 mr-4 flex-shrink-0" fill="none"
                    stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z">
                    </path>
                  </svg>
                  <div>
                    <p class="font-semibold text-gray-200 text-lg sm:text-xl mb-1">Phone</p>
                    <a href="tel:+2348132924637" class="text-blue-300 text-base sm:text-lg">
                      +234 813 292 4637
                    </a>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact Form Section -->
    <section class="py-12 sm:py-16 lg:py-20 bg-white">
      <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center mb-8 sm:mb-12">
          <h2 class="text-2xl sm:text-3xl lg:text-4xl font-bold text-gray-900 mb-4">
            Send us a Message
          </h2>
          <p class="text-gray-600 text-sm sm:text-base lg:text-lg max-w-2xl mx-auto">
            Have a question or want to work together? Fill out the form below and we'll get back to you as soon as
            possible.
          </p>
        </div>

        <div class="bg-gray-50 rounded-xl shadow-lg p-6 sm:p-8 lg:p-10">
          <form @submit.prevent="submitForm" class="space-y-6">
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 sm:gap-6">
              <div>
                <label for="firstName" class="block text-sm font-medium text-gray-700 mb-2">
                  First Name *
                </label>
                <input type="text" id="firstName" v-model="form.firstName" required
                  class="w-full px-3 sm:px-4 py-2 sm:py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors text-sm sm:text-base"
                  placeholder="Enter your first name" />
              </div>
              <div>
                <label for="lastName" class="block text-sm font-medium text-gray-700 mb-2">
                  Last Name *
                </label>
                <input type="text" id="lastName" v-model="form.lastName" required
                  class="w-full px-3 sm:px-4 py-2 sm:py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors text-sm sm:text-base"
                  placeholder="Enter your last name" />
              </div>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 sm:gap-6">
              <div>
                <label for="email" class="block text-sm font-medium text-gray-700 mb-2">
                  Email Address *
                </label>
                <input type="email" id="email" v-model="form.email" required
                  class="w-full px-3 sm:px-4 py-2 sm:py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors text-sm sm:text-base"
                  placeholder="Enter your email address" />
              </div>
              <div>
                <label for="phone" class="block text-sm font-medium text-gray-700 mb-2">
                  Phone Number
                </label>
                <input type="tel" id="phone" v-model="form.phone"
                  class="w-full px-3 sm:px-4 py-2 sm:py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors text-sm sm:text-base"
                  placeholder="Enter your phone number" />
              </div>
            </div>

            <div>
              <label for="subject" class="block text-sm font-medium text-gray-700 mb-2">
                Subject *
              </label>
              <input type="text" id="subject" v-model="form.subject" required
                class="w-full px-3 sm:px-4 py-2 sm:py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors text-sm sm:text-base"
                placeholder="What's this about?" />
            </div>

            <div>
              <label for="message" class="block text-sm font-medium text-gray-700 mb-2">
                Message *
              </label>
              <textarea id="message" v-model="form.message" required rows="5"
                class="w-full px-3 sm:px-4 py-2 sm:py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors resize-none text-sm sm:text-base"
                placeholder="Tell us more about your inquiry..."></textarea>
            </div>

            <div class="flex flex-col sm:flex-row gap-4 pt-4">
              <button type="submit" :disabled="isSubmitting"
                class="flex-1 bg-blue-600 text-white py-3 px-6 rounded-lg font-medium hover:bg-blue-700 focus:ring-2 focus:ring-blue-500 focus:ring-offset-2 transition-colors disabled:opacity-50 disabled:cursor-not-allowed text-sm sm:text-base">
                {{ isSubmitting ? 'Sending...' : 'Send Message' }}
              </button>
              <button type="button" @click="resetForm"
                class="flex-1 sm:flex-initial bg-gray-300 text-gray-700 py-3 px-6 rounded-lg font-medium hover:bg-gray-400 focus:ring-2 focus:ring-gray-500 focus:ring-offset-2 transition-colors text-sm sm:text-base">
                Reset
              </button>
            </div>
          </form>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
import { DotLottieVue } from '@lottiefiles/dotlottie-vue'
import { ref } from 'vue'

// Page meta
definePageMeta({
  layout: "landing"
})

// SEO
useHead({
  title: 'Contact Us - Wilson Samson',
  meta: [
    {
      name: 'description',
      content: 'Get in touch with Wilson Samson. Contact us for inquiries, support, or collaboration opportunities.'
    }
  ]
})

// Form data
const form = ref({
  firstName: '',
  lastName: '',
  email: '',
  phone: '',
  subject: '',
  message: ''
})

const isSubmitting = ref(false)

// Form submission
const submitForm = async () => {
  isSubmitting.value = true

  try {
    // Simulate form submission
    await new Promise(resolve => setTimeout(resolve, 1000))

    // Here you would typically send the form data to your backend
    console.log('Form submitted:', form.value)

    // Reset form
    resetForm()

    // Show success message (you can implement a toast notification here)
    alert('Thank you for your message! We\'ll get back to you soon.')

  } catch (error) {
    console.error('Form submission error:', error)
    alert('There was an error sending your message. Please try again.')
  } finally {
    isSubmitting.value = false
  }
}

// Reset form function
const resetForm = () => {
  form.value = {
    firstName: '',
    lastName: '',
    email: '',
    phone: '',
    subject: '',
    message: ''
  }
}
</script>

<style scoped>
/* Additional custom styles if needed */
</style>