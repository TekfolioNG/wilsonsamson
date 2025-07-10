<script setup>
import { onMounted, ref } from 'vue';

const menuitems = [
  { title: "HOME", path: "/", hasDropdown: false },
  { title: "ABOUT WILSON", path: "/about", hasDropdown: false },
  { title: "CLARITY SESSIONS", path: "/clarity-sessions", hasDropdown: false },
  { title: "TRAINING", path: "/training", hasDropdown: false },
  { title: "MY BOOKS", path: "/my-books", hasDropdown: false },
];

const open = ref(false);
const isContactHovered = ref(false);
const isContactClicked = ref(false);

const handleContactHover = (hovering) => {
  isContactHovered.value = hovering;
};

const handleContactClick = () => {
  isContactClicked.value = true;
  setTimeout(() => {
    isContactClicked.value = false;
  }, 1000);
};

// Preload images for faster loading
const preloadImages = () => {
  const imageUrls = [
    '/img/climate-smart-agric.jpg',
    '/img/carbon-sequestration.jpg',
    '/img/ecofuel-briquettes.jpg'
  ];

  imageUrls.forEach(url => {
    const img = new Image();
    img.src = url;
  });
};

onMounted(() => {
  preloadImages();
});
</script>

<template>
  <div class="absolute w-full z-50 top-4 left-0 right-0">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
      <header class="flex items-center justify-between py-4">
        <!-- Logo section -->
        <NuxtLink to="/" class="inline-block ml-4 md:ml-0">
          <img src="/img/wilsonsamson-logo.png" alt="wilsonsamson Logo"
            class="h-18 md:h-24 drop-shadow-lg filter invert brightness-0" />
        </NuxtLink>

        <!-- Desktop Navigation -->
        <div class="hidden md:flex items-center">
          <!-- Centered Nav Items - Shifted left slightly -->
          <nav class="absolute left-[48%] transform -translate-x-1/2">
            <ul class="flex space-x-6 lg:space-x-8">
              <li v-for="item in menuitems" :key="item.title" class="relative">
                <NuxtLink :to="item.path" :class="[
                  'text-sm lg:text-base transition-colors duration-200 flex items-center whitespace-nowrap font-medium text-white/70 hover:text-white',
                  { 'router-link-exact-active': false }
                ]">
                  {{ item.title }}
                </NuxtLink>
              </li>
            </ul>
          </nav>

          <!-- Connect with Me Button with animated effect -->
          <div class="hidden md:flex items-center ml-auto">
            <NuxtLink to="/contact"
              class="px-4 py-2 rounded-md text-sm lg:text-base font-medium whitespace-nowrap transition-all duration-200 mr-12 relative overflow-hidden group"
              :class="[
                'text-white/70 hover:text-white',
                'border border-transparent bg-transparent',
                isContactClicked ? 'animate-pulse scale-95' : ''
              ]" @click="handleContactClick" @mouseenter="handleContactHover(true)"
              @mouseleave="handleContactHover(false)">
              CONNECT WITH ME

              <!-- Animated Border Progress - Default state (visible) -->
              <div class="absolute inset-0 rounded-md pointer-events-none">
                <!-- Top border -->
                <div class="absolute top-0 left-0 h-0.5 rounded-t-md transition-all duration-300 ease-out" :class="[
                  'bg-white/70',
                  !isContactHovered && !isContactClicked ? 'w-full' : 'w-0'
                ]"></div>
                <!-- Right border -->
                <div class="absolute top-0 right-0 w-0.5 rounded-tr-md transition-all duration-300 ease-out delay-75"
                  :class="[
                    'bg-white/70',
                    !isContactHovered && !isContactClicked ? 'h-full' : 'h-0'
                  ]"></div>
                <!-- Bottom border -->
                <div
                  class="absolute bottom-0 right-0 h-0.5 rounded-br-md transition-all duration-300 ease-out delay-150"
                  :class="[
                    'bg-white/70',
                    !isContactHovered && !isContactClicked ? 'w-full' : 'w-0'
                  ]"></div>
                <!-- Left border -->
                <div
                  class="absolute bottom-0 left-0 w-0.5 rounded-bl-md transition-all duration-300 ease-out delay-[225ms]"
                  :class="[
                    'bg-white/70',
                    !isContactHovered && !isContactClicked ? 'h-full' : 'h-0'
                  ]"></div>
              </div>

              <!-- Small dash underneath text on hover -->
              <div class="absolute bottom-0 right-4 h-0.5 bg-white rounded-full transition-all duration-300 ease-out"
                :class="[
                  isContactHovered ? 'w-8 opacity-100' : 'w-0 opacity-0'
                ]"></div>

              <!-- Ripple effect overlay -->
              <span v-if="isContactClicked" class="absolute inset-0 bg-white/20 rounded-md animate-ping"></span>
            </NuxtLink>
          </div>
        </div>

        <!-- Mobile Menu Button -->
        <div class="md:hidden flex items-center">
          <button @click="open = !open" class="focus:outline-none text-white/70 hover:text-white mr-4">
            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path v-show="!open" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16" />
              <path v-show="open" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M6 18L18 6M6 6l12 12" />
            </svg>
          </button>
        </div>
      </header>

      <!-- Mobile Menu -->
      <transition enter-active-class="transition ease-out duration-100" enter-from-class="transform opacity-0 scale-95"
        enter-to-class="transform opacity-100 scale-100" leave-active-class="transition ease-in duration-75"
        leave-from-class="transform opacity-100 scale-100" leave-to-class="transform opacity-0 scale-95">
        <div v-show="open" class="md:hidden mt-2 py-2 rounded-lg shadow-lg bg-white/95">
          <div v-for="item in menuitems" :key="item.title" class="block">
            <NuxtLink :to="item.path"
              class="block px-4 py-3 text-sm font-medium text-gray-900 hover:text-[#E6A619] transition-colors duration-200"
              @click="open = false">
              {{ item.title }}
            </NuxtLink>
          </div>
          <!-- Mobile Connect Button -->
          <div class="px-4 mt-4">
            <NuxtLink to="/contact"
              class="block w-full text-center px-4 py-3 rounded-md text-sm font-medium text-white bg-white/10 hover:bg-white/20 transition-all duration-200 border border-white/30"
              @click="open = false">
              CONNECT WITH ME
            </NuxtLink>
          </div>
        </div>
      </transition>
    </div>
  </div>
</template>

<style scoped>
/* Active link - only for exact matches */
:deep(.router-link-exact-active) {
  color: white !important;
  position: relative;
}

:deep(.router-link-exact-active::after) {
  content: '';
  position: absolute;
  bottom: -4px;
  left: 0;
  width: 100%;
  height: 2px;
  background-color: white;
  animation: underlineGrow 0.3s ease-out;
}

@keyframes underlineGrow {
  from {
    transform: scaleX(0);
  }

  to {
    transform: scaleX(1);
  }
}

/* Hover effect for nav items */
nav ul li a:not(.router-link-exact-active):hover {
  transform: translateY(-2px);
}

/* Prevent non-exact active links from getting the active color */
:deep(.router-link-active:not(.router-link-exact-active)) {
  color: inherit;
  font-weight: inherit;
}

/* Transitions */
a,
button {
  transition-property: color, background-color, border-color, transform, box-shadow;
  transition-duration: 200ms;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
}
</style>