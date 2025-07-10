<template>
    <div class="min-h-screen bg-gray-50">
        <!-- Social Media Icons - Sticky -->
        <LandingSocialMedia />
        <!-- Main Content -->
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">

            <!-- Hero Section -->
            <section class="mb-24 pt-8 lg:pt-28">
                <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-center">
                    <!-- Content Column -->
                    <div class="space-y-6 mx-4 lg:mx-8">
                        <h3
                            class="inline-flex items-center gap-2 bg-gray-200 text-gray-600 px-4 py-2 rounded-lg text-base font-medium opacity-80 pb-2">
                            <Icon name="mdi:lightbulb" class="w-5 h-5" />
                            FROM BURNOUT TO BETTER BUSINESS
                        </h3>
                        <h1 class="text-4xl lg:text-5xl font-bold text-black leading-tight font-barlow-condensed">
                            Do Less, Achieve More as a
                            <span class="text-blue-600">Business Owner or C-Exec</span>
                        </h1>
                        <p class="text-lg text-gray-900 leading-relaxed">
                            Running a business shouldn't feel like a constant uphill climb. Yet many entrepreneurs find
                            themselves buried in day-to-day operations, with little room left for strategy, growth, or
                            rest.
                        </p>
                        <div class="flex flex-col sm:flex-row gap-4">
                            <NuxtLink to="/contact" target="_blank"
                                class="bg-black hover:bg-white border border-gray-500 hover:border-gray-600 text-white hover:text-gray-800 px-6 py-3 rounded-lg font-semibold transition-all duration-300 text-center">
                                Book a Clarity Session
                            </NuxtLink>
                            <a href="https://wa.me/2348132924637"
                                class="border border-gray-600 hover:border-gray-500 text-gray-800 hover:bg-black hover:text-white px-6 py-3 rounded-lg font-semibold transition-all duration-300 text-center">
                                Schedule Discovery Call
                            </a>
                        </div>
                    </div>

                    <!-- Image Column -->
                    <div class="relative group">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105 mx-4 lg:mx-8">
                            <img src="~/assets/img/burnoout-clarity.jpeg" alt="Business clarity and growth"
                                class="w-full h-[400px] object-cover" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300 mx-4 lg:mx-8">
                        </div>
                    </div>
                </div>
            </section>

            <!-- Problem Identification Section -->
            <section class="mb-24">
                <div class="text-center mb-16 mx-4 lg:mx-8">
                    <h2 class="text-3xl lg:text-4xl font-bold text-black mb-6 font-barlow-condensed">
                        Are These Patterns Showing Up in Your Workflow?
                    </h2>
                    <div class="w-24 h-1 bg-gray-800 rounded-full mx-auto"></div>
                </div>

                <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-start">
                    <!-- Left Column - Problem Cards -->
                    <div class="space-y-6 mx-4 lg:mx-8 order-1">
                        <div class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-4">
                                <div class="flex-shrink-0 mt-1">
                                    <Icon name="heroicons:exclamation-triangle" class="w-6 h-6 text-blue-600" />
                                </div>
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Lack of
                                        Direction and Focus</h3>
                                    <p class="text-gray-900 leading-relaxed">You've got ideas, but they're scattered.
                                        You want growth, but aren't sure what to prioritize.</p>
                                </div>
                            </div>
                        </div>

                        <div class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-4">
                                <div class="flex-shrink-0 mt-1">
                                    <Icon name="heroicons:clock" class="w-6 h-6 text-blue-600" />
                                </div>
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Too Much in the
                                        Weeds</h3>
                                    <p class="text-gray-900 leading-relaxed">You're still making every little decision.
                                        There's no space left to breathe, let alone think long-term.</p>
                                </div>
                            </div>
                        </div>

                        <div class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-4">
                                <div class="flex-shrink-0 mt-1">
                                    <Icon name="heroicons:users" class="w-6 h-6 text-blue-600" />
                                </div>
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Team
                                        Productivity Gaps</h3>
                                    <p class="text-gray-900 leading-relaxed">Your staff depends too heavily on you.
                                        Without you in the room, things stall.</p>
                                </div>
                            </div>
                        </div>

                        <div class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-4">
                                <div class="flex-shrink-0 mt-1">
                                    <Icon name="mdi:microphone" class="w-6 h-6 text-blue-600" />
                                </div>
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Unexpressed
                                        Thought Leadership</h3>
                                    <p class="text-gray-900 leading-relaxed">You've got valuable insights, but no time
                                        or plan to share them through content or speaking.</p>
                                </div>
                            </div>
                        </div>

                        <!-- CTA Card -->
                        <div class="bg-gray-900 rounded-2xl p-8 mt-8">
                            <div class="space-y-6 text-gray-50">
                                <h3 class="text-2xl font-bold text-white font-barlow-condensed">Sounds Familiar?</h3>
                                <p class="text-base leading-relaxed">
                                    If you're overwhelmed, unclear about your direction, or simply tired of doing it
                                    all,
                                    our 1-on-1 Clarity and Growth Program is built to help you reset and lead
                                    differently.
                                </p>
                                <NuxtLink to="/contact" target="_blank"
                                    class="w-full bg-white hover:bg-gray-100 text-black px-6 py-3 rounded-lg font-semibold transition-all duration-300">
                                    Let's Find Your Focus
                                </NuxtLink>
                            </div>
                        </div>
                    </div>

                    <!-- Right Column - Wilson Image -->
                    <div class="relative group mx-4 lg:mx-8 order-2">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105 mt-8 sm:mt-12 lg:mt-16">
                            <img src="~/assets/img/wilsonsamson-hero-image3.png" alt="Wilson Samson"
                                class="w-full h-[600px] sm:h-[700px] lg:h-[800px] object-cover" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300 mt-8 sm:mt-12 lg:mt-16">
                        </div>
                    </div>
                </div>
            </section>

            <!-- Solution Section -->
            <section class="mb-24">
                <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-center">
                    <!-- Image Column - Now on left -->
                    <div class="relative group order-2 lg:order-1">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105 mx-4 lg:mx-8">
                            <img src="~/assets/img/clarity-sessions.png" alt="Clarity coaching sessions"
                                class="w-full h-[400px] sm:h-[500px] lg:h-[600px] object-cover" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300 mx-4 lg:mx-8">
                        </div>
                    </div>

                    <!-- Content Column - Now on right -->
                    <div class="space-y-8 mx-4 lg:mx-8 text-center lg:text-left order-1 lg:order-2">
                        <h3 class="text-3xl font-bold text-black font-barlow-condensed">
                            Reset Your Focus with Our Proven 1-on-1 Clarity Sessions
                        </h3>

                        <div class="bg-white rounded-xl shadow-md p-6 border-l-4 border-blue-600">
                            <p class="text-gray-900 leading-relaxed">
                                The Clarity & Growth Accelerator program is not another business seminar. It's a
                                personalized, result-driven engagement that helps you step back, regain focus, and build
                                a real plan that aligns with your goals.
                            </p>
                        </div>

                        <div class="space-y-4">
                            <h4 class="text-xl font-bold text-black font-barlow-condensed">What's Included:</h4>
                            <div class="space-y-3">
                                <div class="flex items-start">
                                    <Icon name="heroicons:user" class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" />
                                    <span class="text-gray-900 leading-relaxed">One-on-one clarity coaching sessions
                                        with Wilson</span>
                                </div>
                                <div class="flex items-start">
                                    <Icon name="mdi:target" class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" />
                                    <span class="text-gray-900 leading-relaxed">Goal-setting and vision-alignment
                                        exercises</span>
                                </div>
                                <div class="flex items-start">
                                    <Icon name="heroicons:cog-6-tooth"
                                        class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" />
                                    <span class="text-gray-900 leading-relaxed">Strategy tools customized to your
                                        specific business</span>
                                </div>
                                <div class="flex items-start">
                                    <Icon name="heroicons:chart-bar"
                                        class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" />
                                    <span class="text-gray-900 leading-relaxed">Simple, actionable plans you can
                                        implement immediately</span>
                                </div>
                                <div class="flex items-start">
                                    <Icon name="heroicons:document-text"
                                        class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" />
                                    <span class="text-gray-900 leading-relaxed">Optional support for content planning or
                                        book strategy</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- How It Works Section -->
            <section class="mb-24">
                <div class="text-center mb-16 mx-4 lg:mx-8">
                    <h3 class="text-3xl lg:text-4xl font-bold text-black mb-6 font-barlow-condensed">
                        How It Works
                    </h3>
                    <div class="w-24 h-1 bg-gray-800 rounded-full mx-auto"></div>
                </div>

                <div class="grid md:grid-cols-3 gap-8 mx-4 lg:mx-8">
                    <div
                        class="bg-white rounded-xl shadow-md p-8 hover:shadow-lg transition-shadow duration-300 text-center">
                        <div class="bg-gray-800 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-6">
                            <span class="text-white font-bold text-xl">1</span>
                        </div>
                        <h4 class="text-xl font-bold text-black mb-4 font-barlow-condensed">Book a Discovery Call</h4>
                        <p class="text-gray-900 leading-relaxed">We'll identify your current challenges and what success
                            looks like for you.</p>
                    </div>

                    <div
                        class="bg-white rounded-xl shadow-md p-8 hover:shadow-lg transition-shadow duration-300 text-center">
                        <div class="bg-gray-700 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-6">
                            <span class="text-white font-bold text-xl">2</span>
                        </div>
                        <h4 class="text-xl font-bold text-black mb-4 font-barlow-condensed">Schedule Your Sessions</h4>
                        <p class="text-gray-900 leading-relaxed">You'll be guided through 2–3 focused clarity sessions,
                            with practical next steps after each.</p>
                    </div>

                    <div
                        class="bg-white rounded-xl shadow-md p-8 hover:shadow-lg transition-shadow duration-300 text-center">
                        <div class="bg-gray-600 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-6">
                            <span class="text-white font-bold text-xl">3</span>
                        </div>
                        <h4 class="text-xl font-bold text-black mb-4 font-barlow-condensed">Implement With Support</h4>
                        <p class="text-gray-900 leading-relaxed">You'll leave with a plan — not just ideas — and get
                            support to follow through if needed.</p>
                    </div>
                </div>
            </section>

            <!-- Testimonial & CTA Section -->
            <section class="mb-16">
                <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-center">
                    <!-- Testimonial -->
                    <div class="space-y-8 mx-4 lg:mx-8">
                        <h3 class="text-3xl font-bold text-black font-barlow-condensed">
                            Client Success Story
                        </h3>
                        <div class="bg-white rounded-xl shadow-md p-6 border-l-4 border-blue-600">
                            <blockquote class="text-lg text-gray-900 italic mb-4 leading-relaxed">
                                "Wilson helped me reconnect with my business vision. I was stuck in the daily grind for
                                years, but after our clarity sessions, I finally had a clear direction — and the
                                confidence to move forward."
                            </blockquote>
                            <div class="font-semibold text-gray-900">— Adewale B., Business Consultant</div>
                        </div>
                    </div>

                    <!-- CTA Card -->
                    <div class="bg-gray-900 text-white rounded-2xl p-8 mx-4 lg:mx-8">
                        <h4 class="text-2xl font-bold mb-6 font-barlow-condensed">Ready to Work With More Clarity?</h4>
                        <p class="text-gray-300 mb-8 leading-relaxed">
                            It starts with one conversation. Find clarity, reclaim your time, and lead with ease.
                        </p>
                        <div class="space-y-4">
                            <button
                                class="w-full bg-white hover:bg-gray-100 text-black px-6 py-3 rounded-lg font-semibold transition-all duration-300 flex items-center justify-center">
                                <Icon name="heroicons:calendar" class="w-5 h-5 mr-2" />
                                <span>Book a Clarity Session</span>
                            </button>
                            <button
                                class="w-full border-2 border-gray-300 hover:border-gray-200 text-gray-300 hover:text-white px-6 py-3 rounded-lg font-semibold transition-all duration-300 flex items-center justify-center">
                                <Icon name="heroicons:phone" class="w-5 h-5 mr-2" />
                                <span>Schedule Discovery Call</span>
                            </button>
                        </div>
                    </div>
                </div>
            </section>

        </div>
    </div>
</template>

<script setup>
// Define page layout
definePageMeta({
    layout: "landing"
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

.fixed>a:nth-child(5) {
    animation-delay: 0.5s;
}

/* Hover effects */
.group:hover .transition-transform {
    transform: scale(1.02);
}

/* Responsive adjustments */
@media (max-width: 768px) {
    .mx-4 {
        margin-left: 1rem;
        margin-right: 1rem;
    }

    .px-4 {
        padding-left: 1rem;
        padding-right: 1rem;
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