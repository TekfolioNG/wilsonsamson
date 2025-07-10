<template>
  <main class="relative w-screen h-screen overflow-hidden bg-gradient-to-br from-slate-900 via-gray-900 to-slate-800">
    <!-- Background Pattern Overlay -->
    <div class="absolute inset-0 opacity-5">
      <div class="absolute inset-0"
        style="background-image: radial-gradient(circle at 20% 50%, rgba(120, 119, 198, 0.3) 0%, transparent 50%), radial-gradient(circle at 80% 50%, rgba(255, 255, 255, 0.1) 0%, transparent 50%);">
      </div>
    </div>

    <!-- Hero Image -->
    <div class="absolute right-8 top-1/2 transform -translate-y-1/2 w-80 h-96 overflow-hidden rounded-lg shadow-2xl">
      <img src="~/assets/img/wilsonsamson-hero-image.png" alt="Wilson Samson"
        class="w-full h-full object-cover object-center opacity-90" />
      <!-- Subtle gradient overlay for better text contrast -->
      <div class="absolute inset-0 bg-gradient-to-l from-transparent via-transparent to-slate-900/20"></div>
    </div>

    <!-- Logo Behind Main Content -->
    <div class="absolute left-1/2 top-1/2 transform -translate-x-1/2 -translate-y-1/2 opacity-15 z-10">
      <img src="~/assets/img/wilsonsamson-logo2.png" alt="Wilson Samson Logo"
        class="w-48 h-48 object-contain filter invert" />
    </div>

    <!-- Main Content -->
    <div class="relative z-20 w-full h-full flex flex-col justify-center px-8 md:px-16 lg:px-24 xl:px-32 pt-16">
      <div class="max-w-2xl">
        <!-- Hero Heading - Static with 3 steps -->
        <div class="hero-heading text-4xl md:text-5xl lg:text-6xl font-black text-white leading-tight mb-6">
          <div class="mb-2">Lead</div>
          <div class="mb-2">with</div>
          <div class="text-blue-500">Clarity</div>
        </div>

        <!-- Animated Description Lines -->
        <div class="space-y-3 mb-10">
          <transition name="fade-up" appear>
            <p v-show="showLine1" class="text-lg md:text-xl text-gray-300 font-light leading-relaxed">
              Clarity sessions that sharpen your focus.
            </p>
          </transition>

          <transition name="fade-up" appear>
            <p v-show="showLine2" class="text-lg md:text-xl text-gray-300 font-light leading-relaxed">
              Training that empowers your team.
            </p>
          </transition>

          <transition name="fade-up" appear>
            <p v-show="showLine3" class="text-lg md:text-xl text-gray-300 font-light leading-relaxed">
              Strategic writing that builds your authority.
            </p>
          </transition>
        </div>

        <!-- CTA Button -->
        <transition name="fade-up" appear>
          <div v-show="showButton" class="flex justify-start">
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
        </transition>
      </div>
    </div>

    <!-- Signature -->
    <div class="absolute bottom-8 left-8 md:left-16 lg:left-24 xl:left-32 z-30">
      <p class="signature-text text-3xl md:text-4xl text-gray-400 opacity-80">
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
import { ref, onMounted } from 'vue'

// Reactive variables for staggered animation
const showLine1 = ref(false)
const showLine2 = ref(false)
const showLine3 = ref(false)
const showButton = ref(false)

// Staggered animation on mount
onMounted(() => {
  setTimeout(() => { showLine1.value = true }, 500)
  setTimeout(() => { showLine2.value = true }, 1000)
  setTimeout(() => { showLine3.value = true }, 1500)
  setTimeout(() => { showButton.value = true }, 2000)
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
}

.w-screen {
  width: 100vw;
  margin-left: calc(-50vw + 50%);
}

/* Fade up animation */
.fade-up-enter-active {
  transition: all 0.8s ease-out;
}

.fade-up-enter-from {
  opacity: 0;
  transform: translateY(30px);
}

.fade-up-enter-to {
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