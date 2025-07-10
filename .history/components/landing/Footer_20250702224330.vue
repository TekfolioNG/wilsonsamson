<template>
  <footer class="bg-gray-100 text-gray-800 pt-12 pb-8 px-6 sm:px-8">
    <div class="container mx-auto">
      <!-- Main Footer -->
      <div class="grid grid-cols-1 md:grid-cols-12 gap-8 mb-12">
        <!-- Column 1: Logo and Text -->
        <div class="md:col-span-4 flex flex-col items-center md:items-start -mt-4">
          <NuxtLink to="/">
            <img src="~/assets/img/wilsonsamson-logo2.png" alt="Wilson Samson Logo"
              class="h-32 md:h-36 drop-shadow-lg" />
          </NuxtLink>

          <p class="text-gray-600 leading-relaxed mb-6 text-center md:text-left">
            THE BUSINESS CONNECTOR
          </p>
          <NuxtLink to="/about"
            class="text-blue-600 hover:text-blue-500 transition-colors text-sm inline-flex items-center">
            About Wilson Samson
            <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" fill="none" viewBox="0 0 24 24"
              stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
            </svg>
          </NuxtLink>
        </div>

        <!-- Column 2: Menu Links -->
        <div class="md:col-span-4 flex flex-col items-center md:items-start">
          <ul class="space-y-3 text-center md:text-left">
            <li>
              <NuxtLink to="/" class="text-gray-600 hover:text-blue-600 transition-colors">
                Home
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/exec-clarity-sessions" class="text-gray-600 hover:text-blue-600 transition-colors">
                Exec Clarity Sessions
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/employee-productivity-training"
                class="text-gray-600 hover:text-blue-600 transition-colors">
                Employee Productivity Training
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/my-books" class="text-gray-600 hover:text-blue-600 transition-colors">
                My Books
              </NuxtLink>
            </li>
          </ul>
        </div>

        <!-- Column 3: Contact Info -->
        <div class="md:col-span-4 flex flex-col items-center md:items-start">
          <ul class="space-y-4 text-center md:text-left">
            <li class="flex flex-col md:flex-row items-center md:items-start">
              <div class="flex items-start mb-2 md:mb-0 md:mr-3">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-blue-600 flex-shrink-0 mt-1" fill="none"
                  viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
                </svg>
              </div>
              <div class="text-gray-600 text-sm">
                <strong class="block text-gray-800 mb-1">Corporate Address:</strong>
                77 Awolowo Way, Ikeja, Lagos, Nigeria
              </div>
            </li>
            <li class="flex flex-col md:flex-row items-center md:items-start">
              <div class="flex items-center mb-2 md:mb-0 md:mr-3">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-blue-600 flex-shrink-0" fill="none"
                  viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
                </svg>
              </div>
              <div class="text-gray-600 text-sm">
                <strong class="block text-gray-800 mb-1">Tel:</strong>
                +234 818 176 6823,
                <br>+234 813 292 4637 (WhatsApp)
              </div>
            </li>
            <li class="flex flex-col md:flex-row items-center md:items-start">
              <div class="flex items-center mb-2 md:mb-0 md:mr-3">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-blue-600 flex-shrink-0" fill="none"
                  viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                </svg>
              </div>
              <div class="text-gray-600 text-sm">
                <strong class="block text-gray-800 mb-1">E-mail:</strong>
                <a href="mailto:info@wilsonsamson.com"
                  class="hover:text-blue-600 transition-colors">info@wilsonsamson.com</a>
              </div>
            </li>
          </ul>
        </div>
      </div>

      <!-- Footer Bottom -->
      <div class="border-t border-gray-300 pt-6">
        <div class="flex flex-col md:flex-row justify-between items-center gap-4">
          <div class="order-2 md:order-1 text-gray-500 text-sm text-center">
            © {{ new Date().getFullYear() }} WILSON SAMSON & Litera-Forge Ltd. All Rights Reserved.
          </div>
          <div class="order-3 text-gray-500 text-sm text-center md:text-right">
            Website Developed by <NuxtLink to="https://tekfol.io" target="_blank"
              class="text-gray-600 hover:text-blue-600 transition-colors">Tekfolio Ltd</NuxtLink>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>