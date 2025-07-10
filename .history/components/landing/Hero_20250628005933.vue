<template>
  <main class="relative w-screen h-screen overflow-hidden bg-gradient-to-br from-slate-900 via-gray-900 to-slate-800">
    <!-- Background Pattern Overlay -->
    <div class="absolute inset-0 opacity-5">
      <div class="absolute inset-0"
        style="background-image: radial-gradient(circle at 20% 50%, rgba(120, 119, 198, 0.3) 0%, transparent 50%), radial-gradient(circle at 80% 50%, rgba(255, 255, 255, 0.1) 0%, transparent 50%);">
      </div>
    </div>

    <!-- Hero Image - Mobile friendly positioning -->
    <div class="absolute left-0 md:right-0 top-0 w-1/2 md:w-1/2 h-2/5 md:h-full overflow-hidden">
      <img src="/img/wilsonsamson-hero-image.png" alt="Wilson Samson"
        class="w-full h-full object-cover object-center opacity-90" />
      <!-- Enhanced gradient overlay for mobile text contrast -->
      <div
        class="absolute inset-0 bg-gradient-to-r md:bg-gradient-to-l from-transparent via-slate-900/40 md:via-transparent to-slate-900/80 md:to-slate-900/20">
      </div>
    </div>

    <!-- Enhanced Logo Behind Main Content -->
    <div class="absolute left-8 md:left-150 top-3/4 md:top-1/2 transform -translate-y-1/2 z-10 logo-container">
      <img src="~/assets/img/wilsonsamson-logo2.png" alt="Wilson Samson Logo"
        class="logo-enhanced w-32 h-32 md:w-56 md:h-56 object-contain" />
    </div>

    <!-- Main Content - Mobile responsive layout -->
    <div
      class="relative z-20 w-full h-full flex flex-col justify-center md:justify-center px-4 sm:px-6 md:px-16 lg:px-24 xl:px-32">
      <div class="max-w-3xl mt-8 md:mt-16 text-center md:text-left">
        <!-- Hero Heading - Mobile responsive sizing -->
        <h1
          class="hero-heading text-5xl sm:text-6xl md:text-6xl lg:text-7xl xl:text-8xl font-black text-white leading-tight mb-6 md:mb-12">
          Lead with
          <span class="text-blue-500 block">Clarity</span>
        </h1>

        <!-- Single Sliding Description Line - Mobile responsive -->
        <div class="relative h-12 md:h-16 mb-8 md:mb-12">
          <transition name="fade-only" mode="out-in">
            <p v-if="slides[currentSlide].description" :key="currentSlide"
              class="hero-description absolute top-0 left-1/2 md:left-0 transform -translate-x-1/2 md:translate-x-0 text-lg sm:text-xl md:text-2xl text-white max-w-2xl font-normal leading-relaxed"
              style="text-shadow: 0 2px 4px rgba(0,0,0,0.8), 0 0 8px rgba(0,0,0,0.5);">
              {{ slides[currentSlide].description }}
            </p>
          </transition>
        </div>

        <!-- CTA Button - Mobile responsive -->
        <div class="flex justify-center md:justify-start">
          <NuxtLink to="/contact"
            class="group relative inline-flex items-center px-6 md:px-8 py-3 md:py-4 text-base md:text-lg font-semibold text-white bg-blue-600 hover:bg-blue-700 rounded-lg transition-all duration-300 transform hover:scale-105 hover:shadow-2xl">
            <span class="relative z-10 text-center">Start Here to Lead Smarter, Grow Faster</span>
            <div
              class="absolute inset-0 bg-gradient-to-r from-blue-600 to-indigo-600 rounded-lg opacity-0 group-hover:opacity-100 transition-opacity duration-300">
            </div>
            <svg class="ml-2 md:ml-3 w-4 h-4 md:w-5 md:h-5 transition-transform duration-300 group-hover:translate-x-1"
              fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3">
              </path>
            </svg>
          </NuxtLink>
        </div>
      </div>
    </div>

    <!-- Signature - Mobile responsive positioning -->
    <div class="absolute bottom-4 right-4 md:bottom-8 md:right-8 lg:right-16 xl:right-24 2xl:right-32 z-30">
      <p class="signature-text text-xl sm:text-2xl md:text-3xl lg:text-4xl text-white opacity-90">
        Wilson Samson
      </p>
    </div>

    <!-- Decorative Elements - Hidden on mobile for cleaner look -->
    <div class="hidden md:block absolute top-1/4 left-1/4 w-2 h-2 bg-blue-500 rounded-full opacity-60 animate-pulse">
    </div>
    <div class="hidden md:block absolute top-3/4 left-1/3 w-1 h-1 bg-white rounded-full opacity-40 animate-pulse"
      style="animation-delay: 1s;"></div>
    <div class="hidden md:block absolute top-1/2 left-1/5 w-1.5 h-1.5 bg-blue-400 rounded-full opacity-50 animate-pulse"
      style="animation-delay: 2s;"></div>
  </main>
</template>

<script setup>
import { onMounted, onUnmounted, ref } from 'vue'

// Sliding descriptions
const slides = ref([
  { description: "Clarity sessions that sharpen your focus" },
  { description: "Training that empowers your team" },
  { description: "Strategic writing that builds your authority" }
])

const currentSlide = ref(0)
let slideInterval = null

// Auto-advance slides
const startSlideShow = () => {
  slideInterval = setInterval(() => {
    currentSlide.value = (currentSlide.value + 1) % slides.value.length
  }, 6000) // Change every 6 seconds for proper reading time
}

onMounted(() => {
  // Start slideshow after initial load
  setTimeout(() => {
    startSlideShow()
  }, 1000)
})

onUnmounted(() => {
  if (slideInterval) {
    clearInterval(slideInterval)
  }
})
</script>

<style scoped>
.hero-heading {
  font-family: "Inter", "Segoe UI", system-ui, sans-serif;
  font-weight: 900;
  line-height: 1.1;
  text-shadow: 0 4px 12px rgba(0, 0, 0, 0.5);
}

.signature-text {
  font-family: "Dancing Script", "Brush Script MT", cursive;
  font-weight: 400;
  font-style: italic;
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
}

.w-screen {
  width: 100vw;
  margin-left: calc(-50vw + 50%);
}

/* Enhanced Logo Styles */
.logo-container {
  opacity: 0.25;
  /* Increased from 0.1 to 0.25 */
  transition: opacity 0.3s ease;
}

.logo-enhanced {
  /* Image sharpening techniques */
  image-rendering: -webkit-optimize-contrast;
  image-rendering: crisp-edges;
  image-rendering: pixelated;

  /* Enhanced contrast and brightness */
  filter:
    contrast(1.3)
    /* Increase contrast by 30% */
    brightness(1.2)
    /* Increase brightness by 20% */
    saturate(1.1)
    /* Slight saturation boost */
    drop-shadow(0 0 8px rgba(255, 255, 255, 0.1));
  /* Subtle glow */

  /* Smooth transitions */
  transition: all 0.3s ease;
}

/* Optional hover effect to make logo more visible on interaction */
.logo-container:hover {
  opacity: 0.4;
}

.logo-enhanced:hover {
  filter:
    contrast(1.5) brightness(1.3) saturate(1.2) drop-shadow(0 0 12px rgba(255, 255, 255, 0.2));
}

/* Mobile-specific logo adjustments */
@media (max-width: 768px) {
  .logo-container {
    opacity: 0.15;
    left: 1rem !important;
    top: 75% !important;
  }

  .logo-enhanced {
    filter:
      contrast(1.2) brightness(1.1) saturate(1.05) drop-shadow(0 0 6px rgba(255, 255, 255, 0.08));
  }
}

/* Alternative approach - uncomment if you want the logo more prominent */
/*
.logo-container {
  opacity: 0.4;
  background: radial-gradient(circle, rgba(255,255,255,0.05) 0%, transparent 70%);
  border-radius: 50%;
  padding: 2rem;
}
*/

/* Fade only animation for descriptions - slower for reading time */
.fade-only-enter-active {
  transition: opacity 1.5s ease-out;
}

.fade-only-leave-active {
  transition: opacity 1.0s ease-in;
}

.fade-only-enter-from {
  opacity: 0;
}

.fade-only-leave-to {
  opacity: 0;
}

.fade-only-enter-to {
  opacity: 1;
}

/* Responsive adjustments */
@media (max-width: 768px) {

  /* Mobile layout adjustments */
  .hero-heading {
    font-size: 3rem;
    line-height: 1.1;
    margin-bottom: 1.5rem;
  }

  .signature-text {
    font-size: 1.25rem;
  }

  /* Ensure proper mobile stacking */
  main {
    position: relative;
    height: 100vh;
    overflow-x: hidden;
  }

  /* Mobile content positioning - moved up */
  .relative.z-20 {
    padding-top: 25vh;
    /* Reduced from 40vh to move content up */
    padding-bottom: 2rem;
    height: auto;
    min-height: 75vh;
    /* Increased to give more space */
  }
}

@media (max-width: 640px) {
  .hero-heading {
    font-size: 2.75rem;
    /* Increased from 2rem */
    margin-bottom: 1rem;
  }

  .hero-description {
    font-size: 1rem;
    line-height: 1.4;
  }

  /* Adjust button for mobile */
  .group {
    padding: 0.75rem 1.5rem;
    font-size: 0.875rem;
  }

  /* Mobile signature positioning */
  .signature-text {
    font-size: 1rem;
    bottom: 0.5rem !important;
    right: 0.5rem !important;
  }

  /* Further reduce top padding on smaller screens */
  .relative.z-20 {
    padding-top: 20vh;
  }
}

/* Extra small screens */
@media (max-width: 480px) {
  .hero-heading {
    font-size: 2.5rem;
    /* Increased from 1.75rem */
  }

  .relative.z-20 {
    padding-left: 1rem;
    padding-right: 1rem;
    padding-top: 18vh;
    /* Even less top padding for very small screens */
  }

  .group span {
    font-size: 0.8rem;
  }
}

/* Subtle animations */
@keyframes float {

  0%,
  100% {
    transform: translateY(0px);
  }

  50% {
    transform: translateY(-10px);
  }
}

.hero-heading span {
  animation: float 6s ease-in-out infinite;
  animation-delay: 0.5s;
}

/* Enhanced hover effects */
.group:hover .signature-text {
  color: #3b82f6;
  transition: color 0.3s ease;
}
</style>