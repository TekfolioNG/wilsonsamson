<template>
  <div class="min-h-screen bg-gray-50">
    <LandingSocialMedia />

    <!-- Hero Section -->
    <section class="bg-white py-16">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
          <h1 class="text-4xl font-bold text-gray-900 sm:text-5xl">
            Contact Us
          </h1>
          <p class="mt-4 text-xl text-gray-600 max-w-2xl mx-auto">
            We'd love to hear from you. Get in touch with us today.
          </p>
        </div>
      </div>
    </section>

    <!-- Contact Section -->
    <section class="py-16">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
          <!-- Contact Form -->
          <div class="bg-white rounded-lg shadow-lg p-8">
            <h2 class="text-2xl font-bold text-gray-900 mb-6">Send us a message</h2>
            <form @submit.prevent="submitForm" class="space-y-6">
              <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                <div>
                  <label for="firstName" class="block text-sm font-medium text-gray-700 mb-2">
                    First Name
                  </label>
                  <input type="text" id="firstName" v-model="form.firstName" required
                    class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors"
                    placeholder="Enter your first name" />
                </div>
                <div>
                  <label for="lastName" class="block text-sm font-medium text-gray-700 mb-2">
                    Last Name
                  </label>
                  <input type="text" id="lastName" v-model="form.lastName" required
                    class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors"
                    placeholder="Enter your last name" />
                </div>
              </div>

              <div>
                <label for="email" class="block text-sm font-medium text-gray-700 mb-2">
                  Email Address
                </label>
                <input type="email" id="email" v-model="form.email" required
                  class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors"
                  placeholder="Enter your email address" />
              </div>

              <div>
                <label for="phone" class="block text-sm font-medium text-gray-700 mb-2">
                  Phone Number
                </label>
                <input type="tel" id="phone" v-model="form.phone"
                  class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors"
                  placeholder="Enter your phone number" />
              </div>

              <div>
                <label for="subject" class="block text-sm font-medium text-gray-700 mb-2">
                  Subject
                </label>
                <input type="text" id="subject" v-model="form.subject" required
                  class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors"
                  placeholder="What's this about?" />
              </div>

              <div>
                <label for="message" class="block text-sm font-medium text-gray-700 mb-2">
                  Message
                </label>
                <textarea id="message" v-model="form.message" required rows="5"
                  class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-2 focus:ring-blue-500 focus:border-blue-500 transition-colors resize-none"
                  placeholder="Tell us more about your inquiry..."></textarea>
              </div>

              <button type="submit" :disabled="isSubmitting"
                class="w-full bg-blue-600 text-white py-3 px-6 rounded-lg font-medium hover:bg-blue-700 focus:ring-2 focus:ring-blue-500 focus:ring-offset-2 transition-colors disabled:opacity-50 disabled:cursor-not-allowed">
                {{ isSubmitting ? 'Sending...' : 'Send Message' }}
              </button>
            </form>
          </div>

          <!-- Contact Information -->
          <div class="space-y-8">
            <!-- Contact Details -->
            <div class="bg-white rounded-lg shadow-lg p-8">
              <div class="flex items-center mb-6">
                <div class="w-16 h-16 mr-4">
                  <dotlottie-player src="https://lottie.host/3ee84bbb-612e-4ebb-b558-0d0617467073/9VSKxPEINM.lottie"
                    background="transparent" speed="1" loop autoplay class="w-full h-full"></dotlottie-player>
                </div>
                <h2 class="text-2xl font-bold text-gray-900">Get in Touch</h2>
              </div>

              <div class="space-y-4">
                <div class="flex items-start">
                  <svg class="w-6 h-6 text-blue-600 mt-1 mr-3 flex-shrink-0" fill="none" stroke="currentColor"
                    viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z">
                    </path>
                  </svg>
                  <div>
                    <p class="font-medium text-gray-900">Email</p>
                    <a href="mailto:info@wilsonsamson.com" class="text-blue-600 hover:text-blue-700 transition-colors">
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
                    <p class="font-medium text-gray-900">Phone</p>
                    <div class="space-y-1">
                      <a href="tel:+2348132924637" class="block text-blue-600 hover:text-blue-700 transition-colors">
                        +234 813 292 4637
                      </a>
                      <a href="tel:+2348132924637" class="block text-blue-600 hover:text-blue-700 transition-colors">
                        +234 813 292 4637
                      </a>
                    </div>
                  </div>
                </div>
              </div>
            </div>

            <!-- Location -->
            <div class="bg-white rounded-lg shadow-lg p-8">
              <div class="flex items-center mb-6">
                <div class="w-16 h-16 mr-4">
                  <dotlottie-player src="https://lottie.host/fadaf240-98c6-42fe-a1b2-56777059f554/51q7mWaDJN.lottie"
                    background="transparent" speed="1" loop autoplay class="w-full h-full"></dotlottie-player>
                </div>
                <h2 class="text-2xl font-bold text-gray-900">Our Location</h2>
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
                  <p class="font-medium text-gray-900">Address</p>
                  <p class="text-gray-600 leading-relaxed">
                    11 Adeshina Street, Off Olowu Street,<br>
                    Off Obafemi Awolowo Way,<br>
                    Ikeja, Lagos
                  </p>
                </div>
              </div>
            </div>

            <!-- Business Hours -->
            <div class="bg-white rounded-lg shadow-lg p-8">
              <h3 class="text-xl font-bold text-gray-900 mb-4">Business Hours</h3>
              <div class="space-y-2 text-gray-600">
                <div class="flex justify-between">
                  <span>Monday - Friday</span>
                  <span>9:00 AM - 6:00 PM</span>
                </div>
                <div class="flex justify-between">
                  <span>Saturday</span>
                  <span>10:00 AM - 4:00 PM</span>
                </div>
                <div class="flex justify-between">
                  <span>Sunday</span>
                  <span>Closed</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
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