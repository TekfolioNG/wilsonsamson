<template>
  <main class="relative w-screen h-screen overflow-hidden bg-gradient-to-br from-slate-900 via-gray-900 to-slate-800">
    <!-- Background Pattern Overlay -->
    <div class="absolute inset-0 opacity-5">
      <div class="absolute inset-0"
        style="background-image: radial-gradient(circle at 20% 50%, rgba(120, 119, 198, 0.3) 0%, transparent 50%), radial-gradient(circle at 80% 50%, rgba(255, 255, 255, 0.1) 0%, transparent 50%);">
      </div>
    </div>

    <!-- Hero Image -->
    <div class="absolute right-0 top-0 w-1/2 h-full overflow-hidden">
      <img src="/img/wilsonsamson-hero-image.png" alt="Wilson Samson"
        class="w-full h-full object-cover object-center opacity-90" />
      <!-- Subtle gradient overlay for better text contrast -->
      <div class="absolute inset-0 bg-gradient-to-l from-transparent via-transparent to-slate-900/20"></div>
    </div>

    <!-- Logo Behind Main Content -->
    <div class="absolute right-8 top-1/2 transform -translate-y-1/2 opacity-10 z-10">
      <img src="~/assets/img/wilsonsamson-logo2.png" alt="Wilson Samson Logo" class="w-96 h-96 object-contain" />
    </div>

    <!-- Main Content -->
    <div class="relative z-20 w-full h-full flex flex-col justify-center px-8 md:px-16 lg:px-24 xl:px-32">
      <div class="max-w-3xl mt-16">
        <!-- Hero Heading - Moved down -->
        <h1 class="hero-heading text-5xl md:text-6xl lg:text-7xl xl:text-8xl font-black text-white leading-tight mb-12">
          Lead with
          <span class="text-blue-500 block">Clarity</span>
        </h1>

        <!-- Single Sliding Description Line -->
        <div class="relative h-16 mb-12">
          <transition name="fade-only" mode="out-in">
            <p v-if="slides[currentSlide].description" :key="currentSlide"
              class="hero-description absolute top-0 left-0 text-xl md:text-2xl text-white max-w-2xl font-normal leading-relaxed"
              style="text-shadow: 0 2px 4px rgba(0,0,0,0.8), 0 0 8px rgba(0,0,0,0.5);">
              {{ slides[currentSlide].description }}
            </p>
          </transition>
        </div>

        <!-- CTA Button -->
        <div class="flex justify-start">
          <NuxtLink to="/contact"
            class="group relative inline-flex items-center px-8 py-4 text-lg font-semibold text-white bg-blue-600 hover:bg-blue-700 rounded-lg transition-all duration-300 transform hover:scale-105 hover:shadow-2xl">
            <span class="relative z-10">Start Here to Lead Smarter, Grow Faster</span>
            <div
              class="absolute inset-0 bg-gradient-to-r from-blue-600 to-indigo-600 rounded-lg opacity-0 group-hover:opacity-100 transition-opacity duration-300">
            </div>
            <svg class="ml-3 w-5 h-5 transition-transform duration-300 group-hover:translate-x-1" fill="none"
              stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3">
              </path>
            </svg>
          </NuxtLink>
        </div>
      </div>
    </div>

    <!-- Signature - Moved to extreme right and made white -->
    <div class="absolute bottom-8 right-8 md:right-16 lg:right-24 xl:right-32 z-30">
      <p class="signature-text text-3xl md:text-4xl text-white opacity-90">
        Wilson Samson
      </p>
    </div>

    <!-- Decorative Elements -->
    <div class="absolute top-1/4 left-1/4 w-2 h-2 bg-blue-500 rounded-full opacity-60 animate-pulse"></div>
    <div class="absolute top-3/4 left-1/3 w-1 h-1 bg-white rounded-full opacity-40 animate-pulse"
      style="animation-delay: 1s;"></div>
    <div class="absolute top-1/2 left-1/5 w-1.5 h-1.5 bg-blue-400 rounded-full opacity-50 animate-pulse"
      style="animation-delay: 2s;"></div>
  </main>
</template>

<script setup>
import { onMounted, onUnmounted, ref } from 'vue'

// Sliding descriptions
const slides = ref([
  { description: "Clarity sessions that sharpen your focus." },
  { description: "Training that empowers your team." },
  { description: "Strategic writing that builds your authority." }
])

const currentSlide = ref(0)
let slideInterval = null

// Auto-advance slides
const startSlideShow = () => {
  slideInterval = setInterval(() => {
    currentSlide.value = (currentSlide.value + 1) % slides.value.length
  }, 3000) // Change every 3 seconds
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

/* Slide fade animation for descriptions */
.slide-fade-enter-active {
  transition: all 0.8s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.6s ease-in;
}

.slide-fade-enter-from {
  opacity: 0;
  transform: translateY(20px);
}

.slide-fade-leave-to {
  opacity: 0;
  transform: translateY(-20px);
}

.slide-fade-enter-to {
  opacity: 1;
  transform: translateY(0);
}

/* Responsive adjustments */
@media (max-width: 768px) {
  .hero-heading {
    font-size: 3rem;
  }

  main {
    flex-direction: column;
  }

  .signature-text {
    font-size: 1.5rem;
  }
}

@media (max-width: 640px) {
  .hero-heading {
    font-size: 2.5rem;
  }

  /* Stack content on mobile */
  main>div:first-child {
    width: 100%;
    height: 40%;
    position: relative;
  }

  main>div:last-child {
    width: 100%;
    padding: 1rem;
  }

  /* Move signature to bottom left on mobile for better visibility */
  .signature-text {
    position: absolute;
    bottom: 8px;
    left: 8px;
    right: auto;
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