<template>
  <footer class="bg-blue-50 text-slate-700 pt-16 pb-8 px-6 sm:px-8">
    <div class="container mx-auto">
      <!-- Main Footer -->
      <div class="space-y-8 mb-12">
        <!-- Row 1: Logo and Tagline -->
        <div class="flex flex-col md:flex-row items-center md:items-center gap-6">
          <NuxtLink to="/">
            <img src="~/assets/img/wilsonsamson-logo2.png" alt="Wilson Samson Logo"
              class="h-24 md:h-28 drop-shadow-lg" />
          </NuxtLink>

          <h2 class="text-2xl md:text-3xl font-bold text-blue-700 text-center md:text-left">
            THE BUSINESS CONNECTOR
          </h2>
        </div>

        <!-- Row 2: Navigation Menu -->
        <div class="flex justify-center md:justify-start">
          <ul class="flex flex-wrap justify-center md:justify-start gap-6 md:gap-8 text-center md:text-left">
            <li>
              <NuxtLink to="/" class="text-slate-600 hover:text-blue-700 transition-colors font-medium">
                Home
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/exec-clarity-sessions"
                class="text-slate-600 hover:text-blue-700 transition-colors font-medium">
                Exec Clarity Sessions
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/employee-productivity-training"
                class="text-slate-600 hover:text-blue-700 transition-colors font-medium">
                Employee Productivity Training
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/my-books" class="text-slate-600 hover:text-blue-700 transition-colors font-medium">
                My Books
              </NuxtLink>
            </li>
          </ul>
        </div>

        <!-- Row 3: About Link -->
        <div class="flex justify-center md:justify-start">
          <NuxtLink to="/about"
            class="text-blue-700 hover:text-blue-800 transition-colors text-sm inline-flex items-center font-medium">
            About Wilson Samson
            <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 ml-1" fill="none" viewBox="0 0 24 24"
              stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
            </svg>
          </NuxtLink>
        </div>

        <!-- Row 4: Contact Info -->
        <div class="grid grid-cols-1 md:grid-cols-3 gap-6 pt-4">
          <!-- Address -->
          <div class="flex items-start justify-center md:justify-start">
            <div class="flex items-start">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-blue-600 flex-shrink-0 mt-1 mr-3" fill="none"
                viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
              </svg>
              <div class="text-slate-600 text-sm text-center md:text-left">
                <strong class="block text-slate-800 mb-1">Corporate Address:</strong>
                77 Awolowo Way, Ikeja, Lagos, Nigeria
              </div>
            </div>
          </div>

          <!-- Phone & WhatsApp -->
          <div class="flex flex-col gap-4">
            <!-- Phone -->
            <div class="flex items-center justify-center md:justify-start">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-blue-600 flex-shrink-0 mr-3" fill="none"
                viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
              </svg>
              <div class="text-slate-600 text-sm text-center md:text-left">
                <strong class="text-slate-800">Tel:</strong> +234 818 176 6823
              </div>
            </div>

            <!-- WhatsApp -->
            <div class="flex items-center justify-center md:justify-start">
              <svg class="h-5 w-5 text-green-500 flex-shrink-0 mr-3" viewBox="0 0 24 24" fill="currentColor">
                <path
                  d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893A11.821 11.821 0 0020.885 3.488" />
              </svg>
              <div class="text-slate-600 text-sm text-center md:text-left">
                <strong class="text-slate-800">WhatsApp:</strong>
                <a href="https://wa.me/2348132924637" target="_blank"
                  class="hover:text-blue-700 transition-colors ml-1">+234 813 292 4637</a>
              </div>
            </div>
          </div>

          <!-- Email -->
          <div class="flex items-center justify-center md:justify-start">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-blue-600 flex-shrink-0 mr-3" fill="none"
              viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
            </svg>
            <div class="text-slate-600 text-sm text-center md:text-left">
              <strong class="text-slate-800">E-mail:</strong>
              <a href="mailto:info@wilsonsamson.com"
                class="hover:text-blue-700 transition-colors ml-1">info@wilsonsamson.com</a>
            </div>
          </div>
        </div>
      </div>

      <!-- Footer Bottom -->
      <div class="border-t border-blue-200 pt-6">
        <div class="flex flex-col md:flex-row justify-between items-center gap-4">
          <div class="order-2 md:order-1 text-slate-500 text-sm text-center">
            © {{ new Date().getFullYear() }} WILSON SAMSON & Litera-Forge Ltd. All Rights Reserved.
          </div>
          <div class="order-3 text-slate-500 text-sm text-center md:text-right">
            Website Developed by <NuxtLink to="https://tekfol.io" target="_blank"
              class="text-slate-600 hover:text-blue-700 transition-colors">Tekfolio Ltd</NuxtLink>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>