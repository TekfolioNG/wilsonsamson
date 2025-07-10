<template>
    <div class="min-h-screen bg-gray-50">
        <!-- Social Media Icons - Sticky -->
        <div class="fixed right-6 top-1/2 transform -translate-y-1/2 z-50 flex flex-col gap-4 hidden lg:flex">
            <a v-for="(social, index) in socialLinks" :key="social.name" :href="social.url" target="_blank"
                rel="noopener noreferrer"
                class="w-12 h-12 flex items-center justify-center transition-all duration-300 hover:scale-110 hover:shadow-lg opacity-80 hover:opacity-100 shadow-md rounded-full bg-white"
                :style="{ animationDelay: `${index * 100}ms` }" @mouseenter="social.isHovered = true"
                @mouseleave="social.isHovered = false">
                <Icon v-if="social.name !== 'Twitter' && social.name !== 'TikTok'" :name="social.icon" class="w-6 h-6"
                    :class="social.colorClass" />
                <img v-else-if="social.name === 'Twitter'" src="/assets/img/x-logo.png" alt="X" class="w-5 h-5" />
                <img v-else-if="social.name === 'TikTok'" src="/assets/img/tiktok-logo2.png" alt="TikTok"
                    class="w-5 h-5" />
            </a>
        </div>

        <!-- Mobile Social Media Icons -->
        <div class="lg:hidden flex justify-center gap-4 pt-24 pb-4">
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

        <!-- Main Content -->
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
            <!-- Section 1 -->
            <section class="mb-24 pt-8 lg:pt-28">
                <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-start">
                    <!-- Image Column -->
                    <div class="relative group">
                        <div class="space-y-4 mb-6">
                            <h1
                                class="text-4xl lg:text-5xl font-bold text-black leading-tight font-barlow-condensed ml-4 lg:ml-8">
                                About Wilson Samson
                            </h1>
                        </div>
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105 mx-4 lg:mx-8">
                            <img src="/assets/img/wilsonsamson-hero-image4.png" alt="Wilson Samson"
                                class="w-full h-[400px] object-cover transition-transform duration-700" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300 mx-4 lg:mx-8 mt-[6rem]">
                        </div>
                    </div>

                    <!-- Content Column -->
                    <div class="space-y-8 mx-4 lg:mx-4 pt-4 lg:pt-16">
                        <p class="text-gray-900 text-lg leading-relaxed">
                            Wilson Samson helps business owners reclaim their time, gain clarity, and lead with purpose.
                            For nearly two decades, he has worked with entrepreneurs and teams to build businesses that
                            don’t depend on constant oversight, freeing leaders to focus on what truly matters.
                        </p>
                        <p class="text-gray-900 text-lg leading-relaxed">
                            He is a <strong>Certified Professional in Enterprise Management (CPEM)</strong> from the
                            Institute for
                            Enterprise Management and Analytics, and a recipient of the <strong>UK’s International Award
                                in
                                Delivering Training (IADT).</strong> He holds a B.Sc. in Psychology from Nnamdi Azikiwe
                            University,
                            Anambra State.
                        </p>
                        <p class="text-gray-900 text-lg leading-relaxed">
                            Wilson offers a unique mix of clarity coaching, employee training, and strategic publishing
                            — helping business owners simplify operations, boost team performance, and grow their
                            authority without burning out.
                        </p>
                    </div>
                </div>
            </section>

            <!-- Section 2 -->
            <section class="mb-16">
                <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-center">
                    <!-- Content Column (Left) -->
                    <div class="lg:order-1 space-y-8 bg-black rounded-2xl p-8 mx-4 lg:mx-8">
                        <div class="space-y-6 text-base text-white leading-relaxed">
                            <p>
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
                                Tony Elumelu Foundation, Jobs Initiative Lagos (JIL), Youth Employment Agency (YEA)
                                Ghana, and others.
                            </p>
                        </div>
                    </div>

                    <!-- Image Column (Right) -->
                    <div class="lg:order-2 relative group">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105 mx-4 lg:mx-8">
                            <img src="/assets/img/wilsonsamson-about.jpg" alt="Wilson Samson Professional"
                                class="w-full h-[400px] object-cover filter grayscale transition-all duration-700 group-hover:grayscale-0" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300 mx-4 lg:mx-8">
                        </div>
                    </div>
                </div>

                <!-- Additional company info below the text column -->
                <div class="lg:grid lg:grid-cols-2 gap-12 lg:gap-16 mt-6">
                    <div class="lg:order-1rounded-2xl p-6 mx-4 lg:mx-8">
                        <p class="text-base text-black leading-relaxed">
                            <em>Wilson Samson currently serves as <strong class="text-blue-400">Chief Growth Officer
                                    and
                                    co-founder of Litera-Forge Ltd</strong>, a company he runs alongside his wife,
                                Abimbola.
                            </em>
                        </p>
                    </div>
                    <div class="lg:order-2"></div> <!-- Empty space to maintain alignment -->
                </div>
            </section>

            <!-- Core Values Section -->
            <section class="mb-16">
                <!-- Mobile Heading (shows first on mobile) -->
                <div class="lg:hidden text-center mb-8 px-4">
                    <h2 class="text-4xl font-bold text-black mb-6 font-barlow-condensed">
                        Core Values
                    </h2>
                    <div class="w-24 h-1 bg-gray-800 rounded-full mx-auto mb-8"></div>
                    <p class="text-lg text-gray-900 leading-relaxed">
                        Wilson's work is shaped by clear values that guide how he works and what he helps his
                        clients achieve:
                    </p>
                </div>

                <div class="grid lg:grid-cols-4 gap-8 px-4 lg:px-12">
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

                    <!-- Desktop Heading Column (hidden on mobile) -->
                    <div class="hidden lg:flex flex-col justify-center">
                        <h2 class="text-4xl lg:text-5xl font-bold text-black mb-6 font-barlow-condensed text-right">
                            Core Values
                        </h2>
                        <div class="w-24 h-1 bg-gray-800 rounded-full ml-auto mb-8"></div>
                        <p class="text-lg text-gray-900 leading-relaxed text-right">
                            Wilson's work is shaped by clear values that guide how he works and what he helps his
                            clients achieve:
                        </p>
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
        url: 'https://www.linkedin.com/in/wilson-samson/',
        colorClass: 'text-blue-600',
        isHovered: false
    },
    {
        name: 'Twitter',
        icon: 'mdi:twitter',
        url: 'https://x.com/WilsonUchennaS1',
        colorClass: 'text-black',
        isHovered: false
    },
    {
        name: 'Facebook',
        icon: 'mdi:facebook',
        url: 'https://web.facebook.com/people/The-Business-Companion/100088190574699/',
        colorClass: 'text-blue-600',
        isHovered: false
    },
    {
        name: 'Instagram',
        icon: 'mdi:instagram',
        url: 'https://www.instagram.com/wilsonusamson/',
        colorClass: 'text-pink-600',
        isHovered: false
    },
    {
        name: 'TikTok',
        icon: 'mdi:tiktok',
        url: 'https://www.tiktok.com/@thebusinesscompanion',
        colorClass: 'text-black',
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
    .marquee-content {
        white-space: normal;
        animation: none;
        padding-left: 0;
    }
}

@media (max-width: 768px) {

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

    .lg\:px-12 {
        padding-left: 3rem;
        padding-right: 3rem;
    }
}
</style>