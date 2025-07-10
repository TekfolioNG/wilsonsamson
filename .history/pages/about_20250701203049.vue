<template>
    <div class="min-h-screen bg-gray-50">
        <!-- Social Media Icons - Sticky -->
        <div class="fixed right-6 top-1/2 transform -translate-y-1/2 z-50 flex flex-col gap-4">
            <a v-for="(social, index) in socialLinks" :key="social.name" :href="social.url" :class="social.colorClass"
                class="w-12 h-12 rounded-full flex items-center justify-center transition-all duration-300 hover:scale-110 hover:shadow-lg opacity-80 hover:opacity-100"
                :style="{ animationDelay: `${index * 100}ms` }" @mouseenter="social.isHovered = true"
                @mouseleave="social.isHovered = false">
                <Icon :name="social.icon" class="w-6 h-6"
                    :class="social.name === 'Facebook' ? 'text-black' : 'text-white'" />
            </a>
        </div>

        <!-- Main Content -->
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
            <!-- Section 1 -->
            <section class="mb-24">
                <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-center">
                    <!-- Image Column -->
                    <div class="relative group">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105">
                            <img src="/assets/img/wilsonsamson-hero-image4.png" alt="Wilson Samson"
                                class="w-full h-[600px] object-cover transition-transform duration-700" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300">
                        </div>
                    </div>

                    <!-- Content Column -->
                    <div class="space-y-8">
                        <div class="space-y-4">
                            <h1 class="text-5xl lg:text-6xl font-bold text-gray-900 leading-tight">
                                Meet
                                <span
                                    class="bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
                                    Wilson
                                </span>
                            </h1>
                            <div class="w-24 h-1 bg-gradient-to-r from-blue-600 to-purple-600 rounded-full"></div>
                        </div>
                        <p>

                            dedicated a decade of his career as a Mechanical Engineer at a leading multinational oil
                            servicing company, where he witnessed firsthand the untapped potential within organizations.
                        </p>
                        <p>
                            During his tenure, he encountered brilliant individuals who possessed extraordinary gifts
                            but struggled to effectively communicate their value to the world. This observation sparked
                            a profound realization about the gap between talent and opportunity.
                        </p>
                        <p>
                            Recognizing this critical need, Wilson made the bold decision to transition from engineering
                            to empowerment, dedicating his expertise to bridging this gap for aspiring professionals and
                            organizations alike.
                        </p>
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
                                Over the past two decades, Wilson has trained and empowered more than <strong
                                    class="text-blue-600">10,000 professionals</strong> across Nigeria, Ghana, Cameroon,
                                Kenya, Zambia, South Africa, Liberia, the United States, and the United Kingdom.
                            </p>
                            <p>
                                His work cuts across multiple sectors, including oil and gas, tech, logistics, real
                                estate,
                                construction, healthcare, education, and non-profits. Wilson is also an alumnus of the
                                <strong class="text-blue-600">SKYE program (GIZ Germany)</strong> and <strong
                                    class="text-blue-600">Daystar Leadership Academy</strong>.
                            </p>
                            <p>
                                He has served as a volunteer facilitator and mentor with organizations such as the
                                <strong class="text-blue-600">Tony Elumelu Foundation</strong>, <strong
                                    class="text-blue-600">Jobs Initiative Lagos (JIL)</strong>, <strong
                                    class="text-blue-600">Youth Employment Agency (YEA) Ghana</strong>, and others. He
                                currently serves as <strong class="text-blue-600">Chief Growth Officer and co-founder of
                                    Litera-Forge Ltd</strong>, a company he runs alongside his wife, Abimbola.
                            </p>
                        </div>
                    </div>

                    <!-- Image Column (Right) -->
                    <div class="lg:order-2 relative group">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105">
                            <img src="/assets/img/wilsonsamson-about.jpg" alt="Wilson Samson Professional"
                                class="w-full h-[600px] object-cover filter grayscale transition-all duration-700 group-hover:grayscale-0" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300">
                        </div>
                    </div>
                </div>
            </section>

            <!-- Core Values Section -->
            <section class="mb-16">
                <div class="max-w-4xl mx-auto text-center mb-12">
                    <h2 class="text-4xl lg:text-5xl font-bold text-gray-900 mb-6">
                        Core
                        <span class="bg-gradient-to-r from-blue-600 to-gray-800 bg-clip-text text-transparent">
                            Values
                        </span>
                    </h2>
                    <div class="w-24 h-1 bg-gradient-to-r from-blue-600 to-gray-800 rounded-full mx-auto mb-8"></div>
                    <p class="text-xl text-gray-700 leading-relaxed">
                        Wilson's work is shaped by clear values that guide how he works and what he helps his clients
                        achieve:
                    </p>
                </div>

                <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8 mb-16">
                    <!-- Clarity -->
                    <div
                        class="bg-white rounded-xl shadow-lg p-8 hover:shadow-xl transition-shadow duration-300 border-l-4 border-blue-500">
                        <div class="flex items-center mb-4">
                            <div class="w-12 h-12 bg-blue-500 rounded-full flex items-center justify-center mr-4">
                                <Icon name="mdi:eye" class="w-6 h-6 text-white" />
                            </div>
                            <h3 class="text-2xl font-bold text-gray-900">Clarity</h3>
                        </div>
                        <p class="text-gray-700 leading-relaxed">
                            Every decision starts with a clear vision, not just busy work. Without clarity, action is
                            just
                            motion.
                        </p>
                    </div>

                    <!-- Ownership -->
                    <div
                        class="bg-white rounded-xl shadow-lg p-8 hover:shadow-xl transition-shadow duration-300 border-l-4 border-gray-800">
                        <div class="flex items-center mb-4">
                            <div class="w-12 h-12 bg-gray-800 rounded-full flex items-center justify-center mr-4">
                                <Icon name="mdi:shield-key" class="w-6 h-6 text-white" />
                            </div>
                            <h3 class="text-2xl font-bold text-gray-900">Ownership</h3>
                        </div>
                        <p class="text-gray-700 leading-relaxed">
                            Systems aren't just about control. They're what give you room to grow and breathe. You don't
                            need to do everything, but you must lead with intent.
                        </p>
                    </div>

                    <!-- Simplicity -->
                    <div
                        class="bg-white rounded-xl shadow-lg p-8 hover:shadow-xl transition-shadow duration-300 border-l-4 border-blue-500">
                        <div class="flex items-center mb-4">
                            <div class="w-12 h-12 bg-blue-500 rounded-full flex items-center justify-center mr-4">
                                <Icon name="mdi:lightning-bolt" class="w-6 h-6 text-white" />
                            </div>
                            <h3 class="text-2xl font-bold text-gray-900">Simplicity</h3>
                        </div>
                        <p class="text-gray-700 leading-relaxed">
                            Build a business that reflects your values, not just your goals. Business growth doesn't
                            need to
                            be complex.
                        </p>
                    </div>

                    <!-- Empowerment -->
                    <div
                        class="bg-white rounded-xl shadow-lg p-8 hover:shadow-xl transition-shadow duration-300 border-l-4 border-gray-800">
                        <div class="flex items-center mb-4">
                            <div class="w-12 h-12 bg-gray-800 rounded-full flex items-center justify-center mr-4">
                                <Icon name="mdi:account-group" class="w-6 h-6 text-white" />
                            </div>
                            <h3 class="text-2xl font-bold text-gray-900">Empowerment</h3>
                        </div>
                        <p class="text-gray-700 leading-relaxed">
                            Teams thrive when they're trusted, trained, and allowed to lead. Real impact comes from
                            helping
                            others stand on their own.
                        </p>
                    </div>

                    <!-- Impact -->
                    <div
                        class="bg-white rounded-xl shadow-lg p-8 hover:shadow-xl transition-shadow duration-300 border-l-4 border-blue-500 md:col-span-2 lg:col-span-1">
                        <div class="flex items-center mb-4">
                            <div class="w-12 h-12 bg-blue-500 rounded-full flex items-center justify-center mr-4">
                                <Icon name="mdi:trending-up" class="w-6 h-6 text-white" />
                            </div>
                            <h3 class="text-2xl font-bold text-gray-900">Impact</h3>
                        </div>
                        <p class="text-gray-700 leading-relaxed">
                            Every strategy should serve people and move results. Your story and expertise can shift
                            industries — if it's shared the right way.
                        </p>
                    </div>
                </div>
            </section>

            <!-- Closing Statement -->
            <div class="text-center py-16">
                <p class="text-2xl lg:text-3xl text-gray-800 font-light leading-relaxed max-w-4xl mx-auto">
                    "Empowering business owners to build sustainable, purpose-driven enterprises that create lasting
                    impact
                    while freeing leaders to focus on what truly matters."
                </p>
                <div
                    class="mt-8 w-32 h-0.5 bg-gradient-to-r from-blue-600 via-gray-800 to-blue-600 mx-auto rounded-full">
                </div>
            </div>
        </div>
    </div>

</template>

<script setup>
import { onMounted, ref } from 'vue'

// Define page layout
definePageMeta({
    layout: "landing"
})

// Define social media links
const socialLinks = ref([
    {
        name: 'LinkedIn',
        icon: 'mdi:linkedin',
        url: '#',
        colorClass: 'bg-blue-500 hover:bg-blue-600',
        isHovered: false
    },
    {
        name: 'Twitter',
        icon: 'mdi:twitter',
        url: '#',
        colorClass: 'bg-black hover:bg-gray-800',
        isHovered: false
    },
    {
        name: 'Facebook',
        icon: 'mdi:facebook',
        url: '#',
        colorClass: 'bg-white hover:bg-gray-100 text-black',
        isHovered: false
    },
    {
        name: 'Instagram',
        icon: 'mdi:instagram',
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