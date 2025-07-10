<template>
  <footer class="bg-blue-50 text-gray-800 pt-12 pb-8 px-6 sm:px-8">
    <div class="container mx-auto">
      <!-- Main Footer -->
      <div class="grid grid-cols-1 md:grid-cols-12 gap-8 mb-12">
        <!-- Column 1: Logo and Text -->
        <div class="md:col-span-5 flex flex-col md:flex-row items-center md:items-start gap-6 -mt-4">
          <NuxtLink to="/">
            <img src="~/assets/img/wilsonsamson-logo2.png" alt="Wilson Samson Logo"
              class="h-32 md:h-36 drop-shadow-lg" />
          </NuxtLink>
          <div class="flex flex-col justify-center">
            <p class="text-blue-800 text-xl font-medium mb-4 hidden md:block">
              THE BUSINESS CONNECTOR
            </p>
            <NuxtLink to="/about"
              class="text-blue-600 hover:text-blue-800 transition-colors text-sm inline-flex items-center">
              About Wilson Samson
              <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" fill="none" viewBox="0 0 24 24"
                stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
              </svg>
            </NuxtLink>
          </div>
        </div>

        <!-- Column 2: Menu Links -->
        <div class="md:col-span-3">
          <div class="flex flex-wrap justify-center md:justify-start gap-4 md:gap-6">
            <NuxtLink to="/" class="text-blue-800 hover:text-blue-600 transition-colors font-medium">
              Home
            </NuxtLink>
            <NuxtLink to="/exec-clarity-sessions"
              class="text-blue-800 hover:text-blue-600 transition-colors font-medium">
              Exec Clarity Sessions
            </NuxtLink>
            <NuxtLink to="/employee-productivity-training"
              class="text-blue-800 hover:text-blue-600 transition-colors font-medium">
              Employee Training
            </NuxtLink>
            <NuxtLink to="/my-books" class="text-blue-800 hover:text-blue-600 transition-colors font-medium">
              My Books
            </NuxtLink>
          </div>
        </div>

        <!-- Column 3: Contact Info -->
        <div class="md:col-span-4">
          <div class="flex flex-col space-y-4">
            <div class="flex items-start">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-blue-600 flex-shrink-0 mt-1" fill="none"
                viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
              </svg>
              <div class="ml-3 text-blue-800 text-sm">
                <strong class="block font-medium">Corporate Address:</strong>
                77 Awolowo Way, Ikeja, Lagos, Nigeria
              </div>
            </div>

            <div class="flex items-center">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-blue-600 flex-shrink-0" fill="none"
                viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
              </svg>
              <div class="ml-3 text-blue-800 text-sm">
                <strong class="block font-medium">Tel:</strong>
                <div class="flex items-center space-x-2">
                  <span>+234 818 176 6823</span>
                </div>
                <div class="flex items-center mt-1">
                  <img src="~/assets/img/whatsapp-logo.png" alt="WhatsApp" class="h-4 w-4 mr-1" />
                  <span>+234 813 292 4637</span>
                </div>
              </div>
            </div>

            <div class="flex items-center">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-blue-600 flex-shrink-0" fill="none"
                viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
              </svg>
              <div class="ml-3 text-blue-800 text-sm">
                <strong class="block font-medium">E-mail:</strong>
                <a href="mailto:info@wilsonsamson.com" class="hover:text-blue-600 transition-colors">
                  info@wilsonsamson.com
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Mobile: THE BUSINESS CONNECTOR text -->
      <div class="md:hidden text-center mb-6">
        <p class="text-blue-800 text-xl font-medium">
          THE BUSINESS CONNECTOR
        </p>
      </div>

      <!-- Footer Bottom -->
      <div class="border-t border-blue-200 pt-6">
        <div class="flex flex-col md:flex-row justify-between items-center gap-4">
          <div class="order-2 md:order-1 text-blue-600 text-sm text-center">
            © {{ new Date().getFullYear() }} WILSON SAMSON & Litera-Forge Ltd. All Rights Reserved.
          </div>
          <div class="order-3 text-blue-600 text-sm text-center md:text-right">
            Website Developed by <NuxtLink to="https://tekfol.io" target="_blank"
              class="text-blue-800 hover:text-blue-600 transition-colors font-medium">Tekfolio Ltd</NuxtLink>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<style scoped>
/* Add WhatsApp logo styling */
img[alt="WhatsApp"] {
  filter: brightness(0) saturate(100%) invert(39%) sepia(98%) saturate(748%) hue-rotate(134deg) brightness(91%) contrast(101%);
}
</style>