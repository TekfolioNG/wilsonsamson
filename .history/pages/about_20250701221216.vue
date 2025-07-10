<template>
    <div class="min-h-screen bg-gray-50">
        <!-- Social Media Icons - Sticky -->
        <div class="fixed right-6 top-1/2 transform -translate-y-1/2 z-50 flex flex-col gap-4">
            <a v-for="(social, index) in socialLinks" :key="social.name" :href="social.url"
                class="w-12 h-12 flex items-center justify-center transition-all duration-300 hover:scale-110 hover:shadow-lg opacity-80 hover:opacity-100 shadow-md rounded-full bg-white"
                :style="{ animationDelay: `${index * 100}ms` }" @mouseenter="social.isHovered = true"
                @mouseleave="social.isHovered = false">
                <Icon :name="social.icon" class="w-6 h-6" :class="social.colorClass" />
            </a>
        </div>

        <!-- Main Content -->
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
            <!-- Section 1 -->
            <section class="mb-24 pt-28">
                <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-center">
                    <!-- Image Column -->
                    <div class="relative group">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105 mx-4 lg:mx-8">
                            <img src="/assets/img/wilsonsamson-hero-image4.png" alt="Wilson Samson"
                                class="w-full h-[400px] object-cover transition-transform duration-700" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300 mx-4 lg:mx-8">
                        </div>
                    </div>

                    <!-- Content Column -->
                    <div class="space-y-8 mx-4 lg:mx-8">
                        <div class="space-y-4">
                            <h1 class="text-4xl lg:text-5xl font-bold text-black leading-tight font-barlow-condensed">
                                About Wilson Samson
                            </h1>
                        </div>
                        <p class="text-gray-900 text-base leading-relaxed">
                            Wilson dedicated a decade of his career as a Mechanical Engineer at a leading multinational
                            oil
                            servicing company, where he witnessed firsthand the untapped potential within organizations.
                        </p>
                        <p class="text-gray-900 text-base leading-relaxed">
                            During his tenure, he encountered brilliant individuals who possessed extraordinary gifts
                            but struggled to effectively communicate their value to the world. This observation sparked
                            a profound realization about the gap between talent and opportunity.
                        </p>
                        <p class="text-gray-900 text-base leading-relaxed">
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
                    <!-- Image Column (Left) -->
                    <div class="lg:order-1 relative group">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105 mx-4 lg:mx-8">
                            <img src="/assets/img/wilsonsamson-about.jpg" alt="Wilson Samson Professional"
                                class="w-full h-[400px] object-cover filter grayscale transition-all duration-700 group-hover:grayscale-0" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300 mx-4 lg:mx-8">
                        </div>
                    </div>

                    <!-- Content Column (Right) -->
                    <div class="lg:order-2 space-y-8 bg-black rounded-2xl p-8 mx-4 lg:mx-8">
                        <div class="space-y-6 text-base text-white leading-relaxed">
                            <p class="text-lg text-white font-medium">
                                Over the past two decades, Wilson has trained and empowered more than <strong
                                    class="text-blue-400">10,000 professionals</strong> across Nigeria, Ghana, Cameroon,
                                Kenya, Zambia, South Africa, Liberia, the United States, and the United Kingdom.
                            </p>
                            <p>
                                His work cuts across multiple sectors, including oil and gas, tech, logistics, real
                                estate,
                                construction, healthcare, education, and non-profits. Wilson is also an alumnus of the
                                <strong>SKYE program (GIZ Germany)</strong> and <strong>Daystar Leadership
                                    Academy</strong>.
                            </p>
                            <p>
                                He has served as a volunteer facilitator and mentor with organizations such as the
                                Tony Elumelu Foundation<, Jobs Initiative Lagos (JIL), Youth Employment Agency (YEA)
                                    Ghana, and others. </p>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Additional Info Section -->
            <section class="mb-16">
                <div class="max-w-4xl mx-auto px-4 lg:px-8 text-right">
                    <p class="text-lg text-gray-900 leading-relaxed">
                        Wilson Samson currently serves as <strong class="text-blue-600">Chief Growth Officer and
                            co-founder of Litera-Forge Ltd</strong>, a company he runs alongside his wife, Abimbola.
                    </p>
                </div>
            </section>

            <!-- Core Values Section -->
            <section class="mb-16">
                <div class="grid lg:grid-cols-4 gap-8 px-4 lg:px-8">
                    <!-- Cards Column -->
                    <div class="lg:col-span-3">
                        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
                            <!-- Clarity -->
                            <div
                                class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300">
                                <div class="mb-4">
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Clarity</h3>
                                </div>
                                <p class="text-gray-900 leading-relaxed text-sm">
                                    Every decision starts with a clear vision, not just busy work. Without clarity,
                                    action is
                                    just motion.
                                </p>
                            </div>

                            <!-- Ownership -->
                            <div
                                class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300">
                                <div class="mb-4">
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Ownership</h3>
                                </div>
                                <p class="text-gray-900 leading-relaxed text-sm">
                                    Systems aren't just about control. They're what give you room to grow and breathe.
                                    You don't
                                    need to do everything, but you must lead with intent.
                                </p>
                            </div>

                            <!-- Simplicity -->
                            <div
                                class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300">
                                <div class="mb-4">
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Simplicity</h3>
                                </div>
                                <p class="text-gray-900 leading-relaxed text-sm">
                                    Build a business that reflects your values, not just your goals. Business growth
                                    doesn't
                                    need to be complex.
                                </p>
                            </div>

                            <!-- Empowerment -->
                            <div
                                class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300">
                                <div class="mb-4">
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Empowerment</h3>
                                </div>
                                <p class="text-gray-900 leading-relaxed text-sm">
                                    Teams thrive when they're trusted, trained, and allowed to lead. Real impact comes
                                    from
                                    helping others stand on their own.
                                </p>
                            </div>

                            <!-- Impact -->
                            <div
                                class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300 md:col-span-2 lg:col-span-1">
                                <div class="mb-4">
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Impact</h3>
                                </div>
                                <p class="text-gray-900 leading-relaxed text-sm">
                                    Every strategy should serve people and move results. Your story and expertise can
                                    shift
                                    industries — if it's shared the right way.
                                </p>
                            </div>
                        </div>
                    </div>

                    <!-- Heading Column -->
                    <div class="flex flex-col justify-center">
                        <h2 class="text-4xl lg:text-5xl font-bold text-black mb-6 font-barlow-condensed text-right">
                            Core Values
                        </h2>
                        <div class="w-24 h-1 bg-gray-800 rounded-full ml-auto mb-8"></div>
                        <p class="text-lg text-gray-900 leading-relaxed text-right">
                            Wilson's work is shaped by clear values that guide how he works and what he helps his
                            clients
                            achieve:
                        </p>
                    </div>
                </div>
            </section>

            <!-- Testimonial Block -->
            <section class="mb-16 py-12 bg-gradient-to-r from-blue-50 to-gray-50 rounded-2xl overflow-hidden">
                <div class="max-w-4xl mx-auto px-4 lg:px-8">
                    <div class="marquee">
                        <div class="marquee-content">
                            <p class="text-xl lg:text-2xl text-gray-800 font-light leading-relaxed text-center italic">
                                "Empowering business owners to build sustainable, purpose-driven enterprises that create
                                lasting
                                impact while freeing leaders to focus on what truly matters."
                            </p>
                        </div>
                    </div>
                </div>
            </section>
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
        colorClass: 'text-blue-600',
        isHovered: false
    },
    {
        name: 'Twitter',
        icon: 'mdi:twitter',
        url: '#',
        colorClass: 'text-black',
        isHovered: false
    },
    {
        name: 'Facebook',
        icon: 'mdi:facebook',
        url: '#',
        colorClass: 'text-blue-600',
        isHovered: false
    },
    {
        name: 'Instagram',
        icon: 'mdi:instagram',
        url: '#',
        colorClass: 'text-pink-600',
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
/* Import Barlow Condensed font */
@import url('https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@400;700&display=swap');

.font-barlow-condensed {
    font-family: 'Barlow Condensed', sans-serif;
}

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

/* Marquee animation for testimonial */
.marquee {
    width: 100%;
    overflow: hidden;
    white-space: nowrap;
}

.marquee-content {
    display: inline-block;
    white-space: nowrap;
    animation: marquee 20s linear infinite;
    padding-left: 100%;
}

@keyframes marquee {
    0% {
        transform: translateX(0);
    }

    100% {
        transform: translateX(-100%);
    }
}

/* Hover effects */
.group:hover .transition-transform {
    transform: scale(1.02);
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

    .marquee-content {
        white-space: normal;
        animation: none;
        padding-left: 0;
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

    /* Mobile responsive margins */
    .mx-4 {
        margin-left: 1rem;
        margin-right: 1rem;
    }

    .px-4 {
        padding-left: 1rem;
        padding-right: 1rem;
    }

    .marquee-content {
        white-space: normal;
        animation: none;
        padding-left: 0;
    }
}

@media (min-width: 1024px) {
    .lg\:mx-8 {
        margin-left: 2rem;
        margin-right: 2rem;
    }

    .lg\:px-8 {
        padding-left: 2rem;
        padding-right: 2rem;
    }
}
</style>