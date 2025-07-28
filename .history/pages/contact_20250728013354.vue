<template>
  <div class="min-h-screen bg-gray-50">
    <LandingSocialMedia />

    <!-- Hero Section -->
    <section class="bg-white py-12 md:py-16 lg:py-20">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
          <h1 class="text-3xl md:text-4xl lg:text-5xl xl:text-6xl font-bold text-gray-900">
            Contact Us
          </h1>
          <p class="mt-4 md:mt-6 text-lg md:text-xl lg:text-2xl text-gray-600 max-w-3xl mx-auto leading-relaxed">
            We'd love to hear from you. Get in touch with us today and let's start a conversation.
          </p>
        </div>
      </div>
    </section>

    <!-- Contact Information Section -->
    <section class="py-12 md:py-16 lg:py-20">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center mb-12 lg:mb-16">
          <h2 class="text-2xl md:text-3xl lg:text-4xl font-bold text-gray-900 mb-4">
            Get in Touch
          </h2>
          <p class="text-lg text-gray-600 max-w-2xl mx-auto">
            Multiple ways to reach us. Choose what works best for you.
          </p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 xl:grid-cols-3 gap-6 lg:gap-8">
          <!-- Contact Details -->
          <div class="bg-white rounded-xl shadow-lg p-6 lg:p-8 hover:shadow-xl transition-shadow duration-300">
            <div class="flex flex-col items-center text-center mb-6">
              <div class="w-20 h-20 lg:w-24 lg:h-24 mb-4">
                <DotLottieVue class="w-full h-full" autoplay loop
                  src="https://lottie.host/3ee84bbb-612e-4ebb-b558-0d0617467073/9VSKxPEINM.lottie" />
              </div>
              <h3 class="text-xl lg:text-2xl font-bold text-gray-900">Contact Details</h3>
            </div>

            <div class="space-y-4 lg:space-y-6">
              <div class="flex items-start">
                <svg class="w-6 h-6 text-blue-600 mt-1 mr-3 flex-shrink-0" fill="none" stroke="currentColor"
                  viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z">
                  </path>
                </svg>
                <div>
                  <p class="font-semibold text-gray-900 mb-1">Email</p>
                  <a href="mailto:info@wilsonsamson.com"
                    class="text-blue-600 hover:text-blue-700 transition-colors duration-200 text-sm lg:text-base">
                    info@wilsonsamson.com
                  </a>
                </div>
              </div>

              <div class="flex items-start">
                <svg class="w-6 h-6 text-blue-600 mt-1 mr-3 flex-shrink-0" fill="none" stroke="currentColor"
                  viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z">
                  </path>
                </svg>
                <div>
                  <p class="font-semibold text-gray-900 mb-1">Phone</p>
                  <div class="space-y-1">
                    <a href="tel:+2348132924637"
                      class="block text-blue-600 hover:text-blue-700 transition-colors duration-200 text-sm lg:text-base">
                      +234 813 292 4637
                    </a>
                    <a href="tel:+2348132924637"
                      class="block text-blue-600 hover:text-blue-700 transition-colors duration-200 text-sm lg:text-base">
                      +234 813 292 4637
                    </a>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <!-- Location -->
          <div class="bg-white rounded-xl shadow-lg p-6 lg:p-8 hover:shadow-xl transition-shadow duration-300">
            <div class="flex flex-col items-center text-center mb-6">
              <div class="w-20 h-20 lg:w-24 lg:h-24 mb-4">
                <DotLottieVue class="w-full h-full" autoplay loop
                  src="https://lottie.host/fadaf240-98c6-42fe-a1b2-56777059f554/51q7mWaDJN.lottie" />
              </div>
              <h3 class="text-xl lg:text-2xl font-bold text-gray-900">Our Location</h3>
            </div>

            <div class="flex items-start">
              <svg class="w-6 h-6 text-blue-600 mt-1 mr-3 flex-shrink-0" fill="none" stroke="currentColor"
                viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"></path>
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path>
              </svg>
              <div>
                <p class="font-semibold text-gray-900 mb-2">Address</p>
                <p class="text-gray-600 leading-relaxed text-sm lg:text-base">
                  11 Adeshina Street, Off Olowu Street,<br>
                  Off Obafemi Awolowo Way,<br>
                  Ikeja, Lagos
                </p>
              </div>
            </div>
          </div>

          <!-- Business Hours -->
          <div
            class="bg-white rounded-xl shadow-lg p-6 lg:p-8 hover:shadow-xl transition-shadow duration-300 md:col-span-2 xl:col-span-1">
            <div class="text-center mb-6">
              <div
                class="w-20 h-20 lg:w-24 lg:h-24 mx-auto mb-4 flex items-center justify-center bg-blue-50 rounded-full">
                <svg class="w-10 h-10 lg:w-12 lg:h-12 text-blue-600" fill="none" stroke="currentColor"
                  viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z">
                  </path>
                </svg>
              </div>
              <h3 class="text-xl lg:text-2xl font-bold text-gray-900">Business Hours</h3>
            </div>

            <div class="space-y-3 text-sm lg:text-base">
              <div class="flex justify-between items-center py-2 border-b border-gray-100">
                <span class="font-medium text-gray-700">Monday - Friday</span>
                <span class="text-gray-600">9:00 AM - 6:00 PM</span>
              </div>
              <div class="flex justify-between items-center py-2 border-b border-gray-100">
                <span class="font-medium text-gray-700">Saturday</span>
                <span class="text-gray-600">10:00 AM - 4:00 PM</span>
              </div>
              <div class="flex justify-between items-center py-2">
                <span class="font-medium text-gray-700">Sunday</span>
                <span class="text-red-600 font-medium">Closed</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact Form Section -->
    <section class="py-12 md:py-16 lg:py-20 bg-white">
      <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center mb-12 lg:mb-16">
          <h2 class="text-2xl md:text-3xl lg:text-4xl font-bold text-gray-900 mb-4">
            Send us a Message
          </h2>
          <p class="text-lg text-gray-600 max-w-2xl mx-auto">
            Have a question or want to work together? Fill out the form below and we'll get back to you as soon as
            possible.
          </p>
        </div>

        <div class="bg-gray-50 rounded-2xl shadow-xl p-6 md:p-8 lg:p-12">
          <form @submit.prevent="submitForm" class="space-y-6 lg:space-y-8">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6 lg:gap-8">
              <div>
                <label for="firstName" class="block text-sm lg:text-base font-semibold text-gray-700 mb-2">
                  First Name *
                </label>
                <input type="text" id="firstName" v-model="form.firstName" required
                  class="w-full px-4 py-3 lg:px-5 lg:py-4 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-all duration-200 text-sm lg:text-base"
                  placeholder="Enter your first name" />
              </div>
              <div>
                <label for="lastName" class="block text-sm lg:text-base font-semibold text-gray-700 mb-2">
                  Last Name *
                </label>
                <input type="text" id="lastName" v-model="form.lastName" required
                  class="w-full px-4 py-3 lg:px-5 lg:py-4 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-all duration-200 text-sm lg:text-base"
                  placeholder="Enter your last name" />
              </div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-6 lg:gap-8">
              <div>
                <label for="email" class="block text-sm lg:text-base font-semibold text-gray-700 mb-2">
                  Email Address *
                </label>
                <input type="email" id="email" v-model="form.email" required
                  class="w-full px-4 py-3 lg:px-5 lg:py-4 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-all duration-200 text-sm lg:text-base"
                  placeholder="Enter your email address" />
              </div>
              <div>
                <label for="phone" class="block text-sm lg:text-base font-semibold text-gray-700 mb-2">
                  Phone Number
                </label>
                <input type="tel" id="phone" v-model="form.phone"
                  class="w-full px-4 py-3 lg:px-5 lg:py-4 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-all duration-200 text-sm lg:text-base"
                  placeholder="Enter your phone number" />
              </div>
            </div>

            <div>
              <label for="subject" class="block text-sm lg:text-base font-semibold text-gray-700 mb-2">
                Subject *
              </label>
              <input type="text" id="subject" v-model="form.subject" required
                class="w-full px-4 py-3 lg:px-5 lg:py-4 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-all duration-200 text-sm lg:text-base"
                placeholder="What's this about?" />
            </div>

            <div>
              <label for="message" class="block text-sm lg:text-base font-semibold text-gray-700 mb-2">
                Message *
              </label>
              <textarea id="message" v-model="form.message" required rows="6"
                class="w-full px-4 py-3 lg:px-5 lg:py-4 border border-gray-300 rounded-xl focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-all duration-200 resize-none text-sm lg:text-base"
                placeholder="Tell us more about your inquiry..."></textarea>
            </div>

            <div class="text-center">
              <button type="submit" :disabled="isSubmitting"
                class="inline-flex items-center justify-center px-8 py-4 lg:px-12 lg:py-5 bg-blue-600 text-white font-semibold rounded-xl hover:bg-blue-700 focus:ring-4 focus:ring-blue-500 focus:ring-offset-2 transition-all duration-200 disabled:opacity-50 disabled:cursor-not-allowed text-sm lg:text-base min-w-[200px]">
                <svg v-if="isSubmitting" class="animate-spin -ml-1 mr-3 h-5 w-5 text-white"
                  xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24">
                  <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
                  <path class="opacity-75" fill="currentColor"
                    d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z">
                  </path>
                </svg>
                {{ isSubmitting ? 'Sending...' : 'Send Message' }}
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
    form.value = {
      firstName: '',
      lastName: '',
      email: '',
      phone: '',
      subject: '',
      message: ''
    }

    // Show success message (you can implement a toast notification here)
    alert('Thank you for your message! We\'ll get back to you soon.')

  } catch (error) {
    console.error('Form submission error:', error)
    alert('There was an error sending your message. Please try again.')
  } finally {
    isSubmitting.value = false
  }
}
</script>

<style scoped>
/* Additional custom styles if needed */
</style>