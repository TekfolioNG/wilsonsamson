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
                            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                    d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z" />
                            </svg>
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
                            <button
                                class="bg-black hover:bg-white border border-gray-500 hover:border-gray-600 text-white hover:text-gray-800 px-6 py-3 rounded-lg font-semibold transition-all duration-300">
                                Book a Clarity Session
                            </button>
                            <button
                                class="border border-gray-600 hover:border-gray-500 text-gray-800 hover:bg-black hover:text-white px-6 py-3 rounded-lg font-semibold transition-all duration-300">
                                Schedule Discovery Call
                            </button>
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
                                    <svg class="w-6 h-6 text-blue-600" fill="none" stroke="currentColor"
                                        viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-2.5L13.732 4c-.77-.833-1.964-.833-2.732 0L3.732 16.5c-.77.833.192 2.5 1.732 2.5z" />
                                    </svg>
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
                                    <svg class="w-6 h-6 text-blue-600" fill="none" stroke="currentColor"
                                        viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
                                    </svg>
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
                                    <svg class="w-6 h-6 text-blue-600" fill="none" stroke="currentColor"
                                        viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M12 4.354a4 4 0 110 5.292M15 21H3v-1a6 6 0 0112 0v1zm0 0h6v-1a6 6 0 00-9-5.197m13.5-9a2.5 2.5 0 11-5 0 2.5 2.5 0 015 0z" />
                                    </svg>
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
                                    <svg class="w-6 h-6 text-blue-600" fill="none" stroke="currentColor"
                                        viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M19 11a7 7 0 01-7 7m0 0a7 7 0 01-7-7m7 7v4m0 0H8m4 0h4m-4-8a3 3 0 01-3-3V5a3 3 0 116 0v6a3 3 0 01-3 3z" />
                                    </svg>
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
                                <button
                                    class="w-full bg-white hover:bg-gray-100 text-black px-6 py-3 rounded-lg font-semibold transition-all duration-300">
                                    Let's Find Your Focus
                                </button>
                            </div>
                        </div>
                    </div>

                    <!-- Right Column - Wilson Image -->
                    <div class="relative group mx-4 lg:mx-8 order-2">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105">
                            <img src="~/assets/img/wilsonsamson-hero-image3.png" alt="Wilson Samson"
                                class="w-full h-[800px] object-cover" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300">
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
                                class="w-full h-[600px] object-cover" />
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
                                    <svg class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" fill="none"
                                        stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z" />
                                    </svg>
                                    <span class="text-gray-900 leading-relaxed">One-on-one clarity coaching sessions
                                        with Wilson</span>
                                </div>
                                <div class="flex items-start">
                                    <svg class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" fill="none"
                                        stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M7 20l4-16m2 16l4-16M6 9h14M4 15h14" />
                                    </svg>
                                    <span class="text-gray-900 leading-relaxed">Goal-setting and vision-alignment
                                        exercises</span>
                                </div>
                                <div class="flex items-start">
                                    <svg class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" fill="none"
                                        stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 002.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 001.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 00-1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 00-2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 00-2.573-1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 00-1.065-2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 001.066-2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z" />
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                                    </svg>
                                    <span class="text-gray-900 leading-relaxed">Strategy tools customized to your
                                        specific business</span>
                                </div>
                                <div class="flex items-start">
                                    <svg class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" fill="none"
                                        stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z" />
                                    </svg>
                                    <span class="text-gray-900 leading-relaxed">Simple, actionable plans you can
                                        implement immediately</span>
                                </div>
                                <div class="flex items-start">
                                    <svg class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" fill="none"
                                        stroke="currentColor" viewBox="0 0 24 24">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                            d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z" />
                                    </svg>
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
                                <svg class="w-5 h-5 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M8 7V3a1 1 0 011-1h6a1 1 0 011 1v4m-7 0h8m-8 0V17a1 1 0 001 1h6a1 1 0 001-1V7m-8 0H6a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V9a2 2 0 00-2-2h-2" />
                                </svg>
                                <span>Book a Clarity Session</span>
                            </button>
                            <button
                                class="w-full border-2 border-gray-300 hover:border-gray-200 text-gray-300 hover:text-white px-6 py-3 rounded-lg font-semibold transition-all duration-300 flex items-center justify-center">
                                <svg class="w-5 h-5 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                                        d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
                                </svg>
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