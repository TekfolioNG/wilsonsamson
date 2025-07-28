<template>
  <div class="min-h-screen bg-gray-50">
    <!-- Social Media Icons - Sticky -->
    <LandingSocialMedia />

    <!-- Main Content -->
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
      <!-- Page Header -->
      <section class="mb-16 pt-8 lg:pt-16">
        <div class="text-center mx-2 sm:mx-4 lg:mx-6">
          <h1 class="text-3xl sm:text-4xl lg:text-5xl font-bold text-black mb-6 font-barlow-condensed">
            Contact <span class="text-blue-600">Wilson Samson</span>
          </h1>
          <div class="w-24 h-1 bg-blue-600 rounded-full mx-auto mb-8"></div>
          <p class="text-base sm:text-lg text-gray-900 max-w-3xl mx-auto leading-relaxed">
            Get in touch for speaking engagements, consulting services, or publishing inquiries.
          </p>
        </div>
      </section>

      <!-- Contact Details -->
      <section class="mb-20">
        <div class="grid md:grid-cols-2 gap-12 max-w-4xl mx-auto">
          <!-- Contact Form -->
          <div class="bg-white rounded-2xl shadow-xl p-8">
            <h2 class="text-2xl font-bold text-gray-900 mb-6 font-barlow-condensed">Send a Message</h2>
            <form class="space-y-6">
              <div>
                <label for="name" class="block text-sm font-medium text-gray-700 mb-1">Name</label>
                <input type="text" id="name" name="name"
                  class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500">
              </div>
              <div>
                <label for="email" class="block text-sm font-medium text-gray-700 mb-1">Email</label>
                <input type="email" id="email" name="email"
                  class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500">
              </div>
              <div>
                <label for="subject" class="block text-sm font-medium text-gray-700 mb-1">Subject</label>
                <input type="text" id="subject" name="subject"
                  class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500">
              </div>
              <div>
                <label for="message" class="block text-sm font-medium text-gray-700 mb-1">Message</label>
                <textarea id="message" name="message" rows="4"
                  class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-blue-500 focus:border-blue-500"></textarea>
              </div>
              <button type="submit"
                class="w-full bg-blue-600 hover:bg-blue-700 text-white px-6 py-3 rounded-lg font-semibold transition-colors duration-300">
                Send Message
              </button>
            </form>
          </div>

          <!-- Contact Information -->
          <div class="space-y-8">
            <!-- Phone -->
            <div class="flex items-start gap-4">
              <div class="w-16 h-16 flex-shrink-0">
                <dotlottie-player src="https://lottie.host/3ee84bbb-612e-4ebb-b558-0d0617467073/9VSKxPEINM.lottie"
                  background="transparent" speed="1" loop autoplay
                  style="width: 100%; height: 100%;"></dotlottie-player>
              </div>
              <div>
                <h3 class="text-xl font-bold text-gray-900 mb-2 font-barlow-condensed">Phone</h3>
                <p class="text-gray-700">+234 813 292 4637</p>
                <p class="text-gray-700">+234 813 292 4637</p>
              </div>
            </div>

            <!-- Email -->
            <div class="flex items-start gap-4">
              <div class="w-16 h-16 flex-shrink-0">
                <dotlottie-player src="https://lottie.host/3ee84bbb-612e-4ebb-b558-0d0617467073/9VSKxPEINM.lottie"
                  background="transparent" speed="1" loop autoplay
                  style="width: 100%; height: 100%;"></dotlottie-player>
              </div>
              <div>
                <h3 class="text-xl font-bold text-gray-900 mb-2 font-barlow-condensed">Email</h3>
                <p class="text-gray-700">info@wilsonsamson.com</p>
              </div>
            </div>

            <!-- Address -->
            <div class="flex items-start gap-4">
              <div class="w-16 h-16 flex-shrink-0">
                <dotlottie-player src="https://lottie.host/fadaf240-98c6-42fe-a1b2-56777059f554/51q7mWaDJN.lottie"
                  background="transparent" speed="1" loop autoplay
                  style="width: 100%; height: 100%;"></dotlottie-player>
              </div>
              <div>
                <h3 class="text-xl font-bold text-gray-900 mb-2 font-barlow-condensed">Office</h3>
                <p class="text-gray-700">
                  11 Adeshina Street,<br>
                  Off Olowu Street,<br>
                  Off Obafemi Awolowo Way,<br>
                  Ikeja, Lagos
                </p>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- Map Section -->
      <section class="mb-16">
        <div class="bg-white rounded-2xl shadow-xl overflow-hidden">
          <div class="h-96 w-full">
            <iframe
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3963.952912260219!2d3.358295414266941!3d6.5276316452784755!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x103b8b2ae68280c1%3A0xdc9e87a367c3d9cb!2sLagos%20Business%20School!5e0!3m2!1sen!2sng!4v1620000000000!5m2!1sen!2sng"
              width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy">
            </iframe>
          </div>
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
  title: 'Contact Wilson Samson - Leadership Consultant & Author',
  meta: [
    {
      name: 'description',
      content: 'Get in touch with Wilson Samson for speaking engagements, consulting services, or publishing inquiries.'
    }
  ]
})

// Load Lottie player script
useHead({
  script: [
    {
      src: 'https://unpkg.com/@dotlottie/player-component@latest/dist/dotlottie-player.mjs',
      type: 'module'
    }
  ]
})
</script>

<style scoped>
/* Custom animations and effects */
* {
  transition-property: color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, backdrop-filter;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 150ms;
}

/* Enhanced responsive design */
@media (max-width: 640px) {
  .mx-2 {
    margin-left: 0.5rem;
    margin-right: 0.5rem;
  }
}

@media (min-width: 640px) and (max-width: 1023px) {
  .sm\:mx-4 {
    margin-left: 1rem;
    margin-right: 1rem;
  }
}

@media (min-width: 1024px) {
  .lg\:mx-6 {
    margin-left: 1.5rem;
    margin-right: 1.5rem;
  }
}

/* Focus styles */
input:focus,
textarea:focus,
button:focus {
  outline: 2px solid #3B82F6;
  outline-offset: 2px;
  ring: 2px;
}
</style>