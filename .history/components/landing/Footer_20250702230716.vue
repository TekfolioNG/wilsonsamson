<template>
  <footer class="bg-blue-100 text-gray-800 py-12 px-6 sm:px-8">
    <div class="container mx-auto max-w-4xl">
      <!-- Main Content - Centered -->
      <div class="flex flex-col items-center text-center">
        <!-- Logo and Title -->
        <div class="flex flex-col md:flex-row items-center gap-4 mb-8">
          <NuxtLink to="/">
            <img src="~/assets/img/wilsonsamson-logo2.png" alt="Wilson Samson Logo" class="h-20 md:h-24" />
          </NuxtLink>
          <p class="text-blue-800 text-lg md:text-xl font-medium">
            THE BUSINESS CONNECTOR
          </p>
        </div>

        <!-- Navigation Links -->
        <div class="flex flex-wrap justify-center gap-4 md:gap-6 mb-10">
          <NuxtLink to="/" class="text-blue-700 hover:text-blue-900 transition-colors font-medium">
            Home
          </NuxtLink>
          <NuxtLink to="/exec-clarity-sessions" class="text-blue-700 hover:text-blue-900 transition-colors font-medium">
            Exec Clarity
          </NuxtLink>
          <NuxtLink to="/employee-productivity-training"
            class="text-blue-700 hover:text-blue-900 transition-colors font-medium">
            Training
          </NuxtLink>
          <NuxtLink to="/my-books" class="text-blue-700 hover:text-blue-900 transition-colors font-medium">
            My Books
          </NuxtLink>
          <NuxtLink to="/about" class="text-blue-700 hover:text-blue-900 transition-colors font-medium">
            About
          </NuxtLink>
        </div>

        <!-- Contact Icons -->
        <div class="flex justify-center space-x-6 mb-10">
          <!-- Phone -->
          <a href="tel:+2348181766823" class="text-blue-700 hover:text-blue-900 transition-colors">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24"
              stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
            </svg>
          </a>

          <!-- WhatsApp -->
          <a href="https://wa.me/2348132924637" class="text-green-600 hover:text-green-800 transition-colors">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" viewBox="0 0 24 24" fill="currentColor">
              <path
                d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-6.29-3.51c.549 1.422 1.444 2.695 2.655 3.602.094.059.19.11.283.159.073.038.139.072.195.1.173.075.347.133.497.195.05.02.095.04.138.058.323.13.486.193.621.186.155-.007.31-.077.452-.219.48-.48.89-1.05 1.191-1.616.22-.405.385-.803.384-1.155 0-.25-.061-.47-.255-.636-.207-.176-.576-.186-.789-.167-.249.023-.5.05-.75.077l-.095.008c-.166.015-.334.03-.5.045-.076.008-.152.015-.227.023-.419.035-.798.066-1.128-.094-.234-.112-.454-.27-.638-.45-.126-.124-.277-.278-.42-.426-.338-.354-.659-.69-.93-1.02-.063-.075-.123-.148-.18-.22-.176-.22-.326-.408-.45-.558-.047-.057-.084-.102-.112-.135-.174-.213-.286-.35-.286-.35s-.174-.223-.26-.334c-.086-.11-.222-.257-.031-.47.192-.212.576-.005.735.106.148.102.257.201.374.31.117.11.238.225.348.33.11.105.213.203.302.29.09.087.165.158.225.213.06.054.102.09.126.108l.007.006c.058.052.112.1.162.145.054.048.105.093.153.135a6.53 6.53 0 01.42.406c.058.07.117.14.173.21.01.013.02.025.03.038z" />
            </svg>
          </a>

          <!-- Email -->
          <a href="mailto:info@wilsonsamson.com" class="text-blue-700 hover:text-blue-900 transition-colors">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24"
              stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
            </svg>
          </a>

          <!-- Location -->
          <a href="https://maps.google.com?q=77+Awolowo+Way,Ikeja,Lagos"
            class="text-blue-700 hover:text-blue-900 transition-colors">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24"
              stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
            </svg>
          </a>
        </div>
      </div>

      <!-- Footer Bottom -->
      <div class="border-t border-blue-200 pt-6 text-center">
        <div class="text-blue-700 text-sm">
          © {{ new Date().getFullYear() }} WILSON SAMSON & Litera-Forge Ltd. All Rights Reserved.
        </div>
        <div class="text-blue-600 text-xs mt-2">
          Website by <NuxtLink to="https://tekfol.io" target="_blank" class="hover:text-blue-800 transition-colors">
            Tekfolio</NuxtLink>
        </div>
      </div>
    </div>
  </footer>
</template>