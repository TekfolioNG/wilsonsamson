<template>
    <div class="min-h-screen bg-gray-50">
      <!-- Social Media Icons - Sticky -->
      <div class="fixed right-6 top-1/2 transform -translate-y-1/2 z-50 flex flex-col gap-4">
        <a
          v-for="(social, index) in socialLinks"
          :key="social.name"
          :href="social.url"
          :class="social.colorClass"
          class="w-12 h-12 rounded-full flex items-center justify-center transition-all duration-300 hover:scale-110 hover:shadow-lg opacity-80 hover:opacity-100"
          :style="{ animationDelay: `${index * 100}ms` }"
          @mouseenter="social.isHovered = true"
          @mouseleave="social.isHovered = false"
        >
          <component :is="social.icon" class="w-6 h-6" :class="social.name === 'Facebook' ? 'text-black' : 'text-white'" />
        </a>
      </div>
  
      <!-- Main Content -->
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
        <!-- Section 1 -->
        <section class="mb-24">
          <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-center">
            <!-- Image Column -->
            <div class="relative group">
              <div class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105">
                <img
                  src="/assets/img/wilsonsamson-hero-image4.png"
                  alt="Wilson Samson"
                  class="w-full h-[600px] object-cover transition-transform duration-700"
                />
              </div>
              <div class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
            </div>
  
            <!-- Content Column -->
            <div class="space-y-8">
              <div class="space-y-4">
                <h1 class="text-5xl lg:text-6xl font-bold text-gray-900 leading-tight">
                  Meet
                  <span class="bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
                    Wilson
                  </span>
                </h1>
                <div class="w-24 h-1 bg-gradient-to-r from-blue-600 to-purple-600 rounded-full"></div>
              </div>
              
              <div class="space-y-6 text-lg text-gray-700 leading-relaxed">
                <p class="text-xl text-gray-800 font-medium">
                  Wilson Samson dedicated a decade of his career as a Mechanical Engineer at a leading multinational oil servicing company, where he witnessed firsthand the untapped potential within organizations.
                </p>
                <p>
                  During his tenure, he encountered brilliant individuals who possessed extraordinary gifts but struggled to effectively communicate their value to the world. This observation sparked a profound realization about the gap between talent and opportunity.
                </p>
                <p>
                  Recognizing this critical need, Wilson made the bold decision to transition from engineering to empowerment, dedicating his expertise to bridging this gap for aspiring professionals and organizations alike.
                </p>
              </div>
            </div>
          </div>
        </section>
  
        <!-- Section 2 -->
        <section class="mb-16">
          <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-center">
            <!-- Content Column (Left) -->
            <div class="lg:order-1 space-y-8">
              <div class="space-y-4">
                <h2 class="text-4xl lg:text-5xl font-bold text-gray-900 leading-tight">
                  Transforming
                  <span class="bg-gradient-to-r from-green-600 to-blue-600 bg-clip-text text-transparent">
                    Potential
                  </span>
                </h2>
                <div class="w-24 h-1 bg-gradient-to-r from-green-600 to-blue-600 rounded-full"></div>
              </div>
              
              <div class="space-y-6 text-lg text-gray-700 leading-relaxed">
                <p class="text-xl text-gray-800 font-medium">
                  Today, Wilson specializes in helping individuals who carry powerful messages but feel uncertain, overwhelmed, or confused about how to share their vision with the world.
                </p>
                <p>
                  Through strategic message clarification and platform development, he enables thought leaders and innovators to amplify their impact while building sustainable, profitable business ecosystems.
                </p>
                <p>
                  Wilson also partners with forward-thinking organizations to cultivate progressive leadership cultures that transform employees into passionate brand ambassadors and equip management teams with cutting-edge communication strategies.
                </p>
              </div>
            </div>
  
            <!-- Image Column (Right) -->
            <div class="lg:order-2 relative group">
              <div class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105">
                <img
                  src="/assets/img/wilsonsamson-about.jpg"
                  alt="Wilson Samson Professional"
                  class="w-full h-[600px] object-cover filter grayscale transition-all duration-700 group-hover:grayscale-0"
                />
              </div>
              <div class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
            </div>
          </div>
        </section>
  
        <!-- Closing Statement -->
        <div class="text-center py-16">
          <p class="text-2xl lg:text-3xl text-gray-800 font-light leading-relaxed max-w-4xl mx-auto">
            "Empowering exceptional individuals and organizations to unlock their full potential through strategic communication, authentic leadership, and purposeful business development."
          </p>
          <div class="mt-8 w-32 h-0.5 bg-gradient-to-r from-blue-600 via-purple-600 to-green-600 mx-auto rounded-full"></div>
        </div>
      </div>
    </div>
  </template>

<script setup>
import { onMounted, ref } from 'vue';

// Define page layout
definePageMeta({
    layout: "landing"
})

// Define social media links
const socialLinks = ref([
    {
        name: 'LinkedIn',
        icon: 'IconLinkedIn',
        url: '#',
        colorClass: 'bg-blue-500 hover:bg-blue-600',
        isHovered: false
    },
    {
        name: 'Twitter',
        icon: 'IconTwitter',
        url: '#',
        colorClass: 'bg-black hover:bg-gray-800',
        isHovered: false
    },
    {
        name: 'Facebook',
        icon: 'IconFacebook',
        url: '#',
        colorClass: 'bg-white hover:bg-gray-100 text-black',
        isHovered: false
    },
    {
        name: 'Instagram',
        icon: 'IconInstagram',
        url: '#',
        colorClass: 'bg-blue-500 hover:bg-blue-600',
        isHovered: false
    }
])

// Animation on mount
onMounted(() => {
    // Add entrance animations
    const sections = document.querySelectorAll('section')
    const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                entry.target.classList.add('animate-fade-in')
            }
        })
    })

    sections.forEach(section => observer.observe(section))
})
</script>

<style scoped>
/* Custom animations */
@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(30px);
    }

    to {
        opacity: 1;
        transform: translateY(0);
    }
}

@keyframes slideInLeft {
    from {
        opacity: 0;
        transform: translateX(-50px);
    }

    to {
        opacity: 1;
        transform: translateX(0);
    }
}

@keyframes slideInRight {
    from {
        opacity: 0;
        transform: translateX(50px);
    }

    to {
        opacity: 1;
        transform: translateX(0);
    }
}

.animate-fade-in {
    animation: fadeIn 0.8s ease-out forwards;
}

/* Social media icons animation */
.fixed>a {
    animation: slideInRight 0.6s ease-out forwards;
    opacity: 0;
}

.fixed>a:nth-child(1) {
    animation-delay: 0.1s;
}

.fixed>a:nth-child(2) {
    animation-delay: 0.2s;
}

.fixed>a:nth-child(3) {
    animation-delay: 0.3s;
}

.fixed>a:nth-child(4) {
    animation-delay: 0.4s;
}

/* Hover effects */
.group:hover .transition-transform {
    transform: scale(1.02);
}

/* Gradient text animation */
.bg-gradient-to-r.bg-clip-text {
    background-size: 200% 200%;
    animation: gradientShift 3s ease infinite;
}

@keyframes gradientShift {
    0% {
        background-position: 0% 50%;
    }

    50% {
        background-position: 100% 50%;
    }

    100% {
        background-position: 0% 50%;
    }
}

/* Responsive adjustments */
@media (max-width: 1024px) {
    .fixed {
        right: 1rem;
    }

    .fixed>a {
        width: 2.5rem;
        height: 2.5rem;
    }
}

@media (max-width: 768px) {
    .fixed {
        position: relative;
        top: auto;
        right: auto;
        transform: none;
        display: flex;
        justify-content: center;
        flex-direction: row;
        gap: 1rem;
        margin: 2rem 0;
    }
}
</style>

<!-- You'll need to create these icon components or use a library like @nuxtjs/icon -->
<!-- Example icon components (you can replace with your preferred icon library) -->
<template>
    <!-- Add these icon components or use @nuxtjs/icon -->
</template>

<script>
// Icon components (replace with your preferred icon solution)
export default {
    components: {
        IconLinkedIn: {
            template: `
          <svg viewBox="0 0 24 24" fill="currentColor">
            <path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/>
          </svg>
        `
        },
        IconTwitter: {
            template: `
          <svg viewBox="0 0 24 24" fill="currentColor">
            <path d="M23.953 4.57a10 10 0 01-2.825.775 4.958 4.958 0 002.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 00-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 00-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 01-2.228-.616v.06a4.923 4.923 0 003.946 4.827 4.996 4.996 0 01-2.212.085 4.936 4.936 0 004.604 3.417 9.867 9.867 0 01-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 007.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0024 4.59z"/>
          </svg>
        `
        },
        IconFacebook: {
            template: `
          <svg viewBox="0 0 24 24" fill="currentColor">
            <path d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"/>
          </svg>
        `
        },
        IconInstagram: {
            template: `
          <svg viewBox="0 0 24 24" fill="currentColor">
            <path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948 0 3.259.014 3.668.072 4.948.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072 3.259 0 3.668-.014 4.948-.072 4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948 0-3.259-.014-3.667-.072-4.947-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.163 6.162 6.163 6.162-2.759 6.162-6.163c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4 0-2.209 1.791-4 4-4s4 1.791 4 4c0 2.21-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/>
          </svg>
        `
        }
    }
}
</script>