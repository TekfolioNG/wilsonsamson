<template>
  <footer class="bg-gray-250 text-gray-900 pt-8 pb-6 px-6 sm:px-8">
    <div class="container mx-auto">
      <!-- Main Footer -->
      <div class="mb-8">
        <!-- Three Grid Layout -->
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8 lg:gap-12">

          <!-- First Column: Logo, Tagline and About Link -->
          <div class="space-y-4">
            <!-- Logo and Tagline -->
            <div class="flex flex-col items-center md:items-start gap-3">
              <NuxtLink to="/">
                <img src="~/assets/img/wilsonsamson-logo2.png" alt="Wilson Samson Logo"
                  class="h-20 md:h-24 drop-shadow-lg" />
              </NuxtLink>

              <div class="text-center md:text-left">
                <h2 class="text-lg md:text-xl font-medium text-blue-600"
                  style="font-family: 'Barlow Condensed', sans-serif;">
                  THE BUSINESS CONNECTOR
                </h2>
              </div>
            </div>

            <!-- About Link -->
            <div class="flex justify-center md:justify-start">
              <NuxtLink to="/about"
                class="text-blue-600 hover:text-blue-700 transition-colors text-base inline-flex items-center font-normal">
                About Wilson Samson
                <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 ml-2 text-blue-600" fill="none"
                  viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
                </svg>
              </NuxtLink>
            </div>
          </div>

          <!-- Second Column: Navigation Menu -->
          <div>
            <nav>
              <ul class="space-y-3">
                <li>
                  <NuxtLink to="/" class="text-gray-900 hover:text-blue-600 transition-colors font-semibold text-base">
                    Home
                  </NuxtLink>
                </li>
                <li>
                  <NuxtLink to="/exec-clarity-sessions"
                    class="text-gray-900 hover:text-blue-600 transition-colors font-semibold text-base">
                    Exec Clarity Sessions
                  </NuxtLink>
                </li>
                <li>
                  <NuxtLink to="/employee-productivity-training"
                    class="text-gray-900 hover:text-blue-600 transition-colors font-semibold text-base">
                    Employee Productivity Training
                  </NuxtLink>
                </li>
                <li>
                  <NuxtLink to="/my-books"
                    class="text-gray-900 hover:text-blue-600 transition-colors font-semibold text-base">
                    My Books
                  </NuxtLink>
                </li>
              </ul>
            </nav>
          </div>

          <!-- Third Column: Contact Info -->
          <div class="space-y-3">
            <!-- Address -->
            <div class="text-gray-900 text-sm">
              77 Awolowo Way, Ikeja, Lagos, Nigeria
            </div>

            <!-- Phone -->
            <div>
              <a href="tel:+2348181766823" class="text-gray-900 hover:text-blue-600 transition-colors text-sm">
                +234 818 176 6823
              </a>
            </div>

            <!-- WhatsApp -->
            <div>
              <a href="https://wa.me/2348132924637" target="_blank"
                class="text-gray-900 hover:text-green-600 transition-colors text-sm">
                +234 813 292 4637
              </a>
            </div>

            <!-- Email -->
            <div>
              <a href="mailto:info@wilsonsamson.com"
                class="text-gray-900 hover:text-blue-600 transition-colors text-sm">
                info@wilsonsamson.com
              </a>
            </div>
          </div>
        </div>
      </div>

      <!-- Footer Bottom -->
      <div class="border-t border-gray-400 pt-4">
        <div class="flex flex-col md:flex-row justify-between items-center gap-2">
          <div class="order-2 md:order-1 text-gray-700 text-xs text-center">
            © {{ new Date().getFullYear() }} WILSON SAMSON & Litera-Forge Ltd. All Rights Reserved.
          </div>
          <div class="order-3 text-gray-700 text-xs text-center md:text-right">
            Website Developed by <NuxtLink to="https://tekfol.io" target="_blank"
              class="text-gray-800 hover:text-gray-900 transition-colors">Tekfolio Ltd</NuxtLink>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>