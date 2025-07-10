<template>
  <section class="relative w-full min-h-screen flex items-center overflow-hidden bg-transparent">
    <!-- Background elements -->
    <div class="absolute inset-0 flex justify-end items-center z-0">
      <!-- Main hero image -->
      <img src="/img/wilsonsamson-hero-image.png" alt="Wilson Samson"
        class="h-[80vh] object-contain object-right mr-8 lg:mr-16" />
      <!-- Secondary logo -->
      <img src="~/assets/img/wilsonsamson-logo2.png" alt="Wilson Samson Logo"
        class="absolute h-32 lg:h-40 right-8 lg:right-16 bottom-1/4 opacity-70" />
    </div>

    <!-- Content -->
    <div class="relative z-10 container mx-auto px-6 lg:px-12 py-24">
      <div class="max-w-2xl">
        <!-- Hero heading with stacked text -->
        <h1 class="text-5xl md:text-6xl lg:text-7xl xl:text-8xl font-bold leading-tight mb-6">
          <span class="block">Lead with</span>
          <span class="block text-[#4285F4]">Clarity.</span>
        </h1>

        <!-- Animated description lines -->
        <div class="space-y-3 mb-10">
          <transition name="fade" mode="out-in">
            <p v-if="showLine1" class="text-lg md:text-xl lg:text-2xl text-gray-700">
              Clarity sessions that sharpen your focus.
            </p>
          </transition>
          <transition name="fade" mode="out-in">
            <p v-if="showLine2" class="text-lg md:text-xl lg:text-2xl text-gray-700">
              Training that empowers your team.
            </p>
          </transition>
          <transition name="fade" mode="out-in">
            <p v-if="showLine3" class="text-lg md:text-xl lg:text-2xl text-gray-700">
              Strategic writing that builds your authority.
            </p>
          </transition>
        </div>

        <!-- CTA Button -->
        <button
          class="px-8 py-4 bg-[#4285F4] text-white font-medium rounded-lg text-lg hover:bg-[#3367D6] transition-all duration-300 transform hover:scale-105 shadow-lg">
          Start Here to Lead Smarter, Grow Faster
        </button>
      </div>

      <!-- Signature at bottom left -->
      <div class="absolute left-6 lg:left-12 bottom-12">
        <p class="font-calligraphic text-3xl text-gray-600">Wilson Samson</p>
      </div>
    </div>
  </section>
</template>

<script setup>
import { onMounted, ref } from 'vue';

const showLine1 = ref(false);
const showLine2 = ref(false);
const showLine3 = ref(false);

onMounted(() => {
  setTimeout(() => { showLine1.value = true; }, 500);
  setTimeout(() => { showLine2.value = true; }, 1500);
  setTimeout(() => { showLine3.value = true; }, 2500);
});
</script>

<style scoped>
/* Font face for calligraphic signature */
@font-face {
  font-family: 'Calligraphic';
  src: url('~/assets/fonts/calligraphic-font.woff2') format('woff2');
  font-weight: normal;
  font-style: normal;
}

.font-calligraphic {
  font-family: 'Calligraphic', cursive;
}

/* Fade transition for description lines */
.fade-enter-active,
.fade-leave-active {
  transition: opacity 1s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}

/* Responsive adjustments */
@media (max-width: 768px) {
  .hero-image {
    opacity: 0.4;
  }

  h1 {
    font-size: 3.5rem;
  }
}

@media (max-width: 640px) {
  h1 {
    font-size: 2.5rem;
  }

  .description-text {
    font-size: 1rem;
  }
}
</style>