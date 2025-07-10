<template>
    <div>
        <!-- Desktop Social Media Icons - Sticky -->
        <div class="fixed right-6 top-1/2 transform -translate-y-1/2 z-50 flex flex-col gap-4 hidden lg:flex">
            <a v-for="(social, index) in socialLinks" :key="social.name" :href="social.url" target="_blank"
                rel="noopener noreferrer"
                class="w-12 h-12 flex items-center justify-center transition-all duration-300 hover:scale-110 hover:shadow-lg opacity-80 hover:opacity-100 shadow-md rounded-full bg-white"
                :style="{ animationDelay: `${index * 100}ms` }">
                <Icon v-if="social.name !== 'Twitter' && social.name !== 'TikTok'" :name="social.icon" class="w-6 h-6"
                    :class="social.colorClass" />
                <img v-else-if="social.name === 'Twitter'" src="/assets/img/x-logo.png" alt="X" class="w-5 h-5" />
                <img v-else-if="social.name === 'TikTok'" src="/assets/img/tiktok-logo2.png" alt="TikTok"
                    class="w-5 h-5" />
            </a>
        </div>

        <!-- Mobile Social Media Icons -->
        <div v-if="showMobile" class="lg:hidden flex justify-center gap-4" :class="mobileClasses">
            <a v-for="(social, index) in socialLinks" :key="social.name" :href="social.url" target="_blank"
                rel="noopener noreferrer"
                class="w-12 h-12 flex items-center justify-center transition-all duration-300 hover:scale-110 hover:shadow-lg opacity-80 hover:opacity-100 shadow-md rounded-full bg-white">
                <Icon v-if="social.name !== 'Twitter' && social.name !== 'TikTok'" :name="social.icon" class="w-6 h-6"
                    :class="social.colorClass" />
                <img v-else-if="social.name === 'Twitter'" src="/assets/img/x-logo.png" alt="X" class="w-5 h-5" />
                <img v-else-if="social.name === 'TikTok'" src="/assets/img/tiktok-logo2.png" alt="TikTok"
                    class="w-5 h-5" />
            </a>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';

// Props
const props = defineProps({
    showMobile: {
        type: Boolean,
        default: true
    },
    mobileClasses: {
        type: String,
        default: 'pt-24 pb-4'
    }
})

// Define social media links
const socialLinks = ref([
    {
        name: 'LinkedIn',
        icon: 'mdi:linkedin',
        url: 'https://www.linkedin.com/in/wilson-samson/',
        colorClass: 'text-blue-600'
    },
    {
        name: 'Twitter',
        icon: 'mdi:twitter',
        url: 'https://x.com/WilsonUchennaS1',
        colorClass: 'text-black'
    },
    {
        name: 'Facebook',
        icon: 'mdi:facebook',
        url: 'https://web.facebook.com/people/The-Business-Companion/100088190574699/',
        colorClass: 'text-blue-600'
    },
    {
        name: 'Instagram',
        icon: 'mdi:instagram',
        url: 'https://www.instagram.com/wilsonusamson/',
        colorClass: 'text-pink-600'
    },
    {
        name: 'TikTok',
        icon: 'mdi:tiktok',
        url: 'https://www.tiktok.com/@thebusinesscompanion',
        colorClass: 'text-black'
    }
])
</script>

<style scoped>
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

.fixed>a:nth-child(5) {
    animation-delay: 0.5s;
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
</style>