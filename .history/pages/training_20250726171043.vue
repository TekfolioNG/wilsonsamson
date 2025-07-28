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
                            class="inline-flex items-center gap-2 bg-blue-100 text-blue-700 px-4 py-2 rounded-lg text-base font-medium opacity-90 pb-2">
                            <Icon name="heroicons:users" class="w-5 h-5" />
                            FROM OVERWORKED TO EMPOWERED
                        </h3>
                        <h1 class="text-4xl lg:text-5xl font-bold text-black leading-tight font-barlow-condensed">
                            Boost Your Business with Our
                            <span class="text-blue-600">Employee Productivity Programs</span>
                        </h1>
                        <p class="text-lg text-gray-900 leading-relaxed">
                            Running a business shouldn't mean handling every task yourself. If your daily operations
                            constantly demand your attention, it's time for a shift that empowers your team and
                            frees you to lead at a higher level.
                        </p>
                        <div class="flex flex-col sm:flex-row gap-4">
                            <NuxtLink to="/contact" target="_blank"
                                class="bg-blue-600 hover:bg-blue-700 text-white px-6 py-3 rounded-lg font-semibold transition-all duration-300 text-center shadow-lg hover:shadow-xl">
                                Transform Your Team
                            </NuxtLink>
                            <a href="https://wa.me/2348132924637"
                                class="border border-blue-600 hover:border-blue-700 text-blue-600 hover:bg-blue-600 hover:text-white px-6 py-3 rounded-lg font-semibold transition-all duration-300 text-center">
                                Get Free Consultation
                            </a>
                        </div>
                    </div>

                    <!-- Image Column -->
                    <div class="relative group">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105 mx-4 lg:mx-8">
                            <img src="~/assets/img/clarity-sessions.png" alt="Employee productivity training"
                                class="w-full h-[400px] object-cover" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-blue-600/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300 mx-4 lg:mx-8">
                        </div>
                    </div>
                </div>
            </section>

            <!-- Problem Identification Section -->
            <section class="mb-24">
                <div class="text-center mb-16 mx-4 lg:mx-8">
                    <h2 class="text-3xl lg:text-4xl font-bold text-black mb-6 font-barlow-condensed">
                        Is Your Team's Potential Being Held Back?
                    </h2>
                    <div class="w-24 h-1 bg-blue-600 rounded-full mx-auto"></div>
                </div>

                <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-start">
                    <!-- Left Column - Problem Cards -->
                    <div class="space-y-6 mx-4 lg:mx-8 order-1">
                        <div
                            class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300 border-l-4 border-red-400">
                            <div class="flex items-start gap-4">
                                <div class="flex-shrink-0 mt-1">
                                    <Icon name="heroicons:arrow-path" class="w-6 h-6 text-red-500" />
                                </div>
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Constant
                                        Micromanagement</h3>
                                    <p class="text-gray-900 leading-relaxed">You're involved in every decision because
                                        your team lacks the confidence or skills to handle tasks independently.</p>
                                </div>
                            </div>
                        </div>

                        <div
                            class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300 border-l-4 border-orange-400">
                            <div class="flex items-start gap-4">
                                <div class="flex-shrink-0 mt-1">
                                    <Icon name="heroicons:clock" class="w-6 h-6 text-orange-500" />
                                </div>
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Inefficient
                                        Workflows</h3>
                                    <p class="text-gray-900 leading-relaxed">Tasks take longer than they should, with
                                        unnecessary back-and-forth and unclear processes.</p>
                                </div>
                            </div>
                        </div>

                        <div
                            class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300 border-l-4 border-yellow-400">
                            <div class="flex items-start gap-4">
                                <div class="flex-shrink-0 mt-1">
                                    <Icon name="heroicons:chat-bubble-left-ellipsis" class="w-6 h-6 text-yellow-600" />
                                </div>
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Communication
                                        Breakdowns</h3>
                                    <p class="text-gray-900 leading-relaxed">Miscommunications lead to errors, delays,
                                        and frustration across your team.</p>
                                </div>
                            </div>
                        </div>

                        <div
                            class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300 border-l-4 border-purple-400">
                            <div class="flex items-start gap-4">
                                <div class="flex-shrink-0 mt-1">
                                    <Icon name="heroicons:user-minus" class="w-6 h-6 text-purple-500" />
                                </div>
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Low Ownership
                                        Mentality</h3>
                                    <p class="text-gray-900 leading-relaxed">Employees wait for instructions instead of
                                        taking initiative, limiting their growth and your business potential.</p>
                                </div>
                            </div>
                        </div>

                        <!-- CTA Card -->
                        <div class="bg-blue-600 rounded-2xl p-8 mt-8">
                            <div class="space-y-6 text-white">
                                <h3 class="text-2xl font-bold font-barlow-condensed">Ready for a Change?</h3>
                                <p class="text-base leading-relaxed text-blue-100">
                                    Transform your team from task-followers to problem-solvers. Our proven Employee
                                    Productivity Programs build the skills and mindset your business needs to thrive.
                                </p>
                                <NuxtLink to="/contact" target="_blank"
                                    class="w-full bg-white hover:bg-gray-100 text-blue-600 px-6 py-3 rounded-lg font-semibold transition-all duration-300 text-center block">
                                    Start the Transformation
                                </NuxtLink>
                            </div>
                        </div>
                    </div>

                    <!-- Right Column - Team Image -->
                    <div class="relative group mx-4 lg:mx-8 order-2">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105 mt-8 sm:mt-12 lg:mt-16">
                            <img src="~/assets/img/wilsonsamson-hero-image3.png" alt="Productive team collaboration"
                                class="w-full h-[600px] sm:h-[700px] lg:h-[800px] object-cover" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-blue-600/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300 mt-8 sm:mt-12 lg:mt-16">
                        </div>
                    </div>
                </div>
            </section>

            <!-- Solution Section -->
            <section class="mb-24">
                <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-center">
                    <!-- Image Column -->
                    <div class="relative group order-2 lg:order-1">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105 mx-4 lg:mx-8">
                            <img src="~/assets/img/burnoout-clarity.jpeg" alt="Employee training and development"
                                class="w-full h-[400px] sm:h-[500px] lg:h-[600px] object-cover" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-blue-600/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300 mx-4 lg:mx-8">
                        </div>
                    </div>

                    <!-- Content Column -->
                    <div class="space-y-8 mx-4 lg:mx-8 text-center lg:text-left order-1 lg:order-2">
                        <h3 class="text-3xl font-bold text-black font-barlow-condensed">
                            What You Get: Complete Team Transformation
                        </h3>

                        <div class="space-y-6">
                            <div class="bg-white rounded-xl shadow-md p-6 border-l-4 border-blue-600">
                                <div class="flex items-start gap-4">
                                    <Icon name="heroicons:cog-6-tooth"
                                        class="w-6 h-6 text-blue-600 mt-1 flex-shrink-0" />
                                    <div>
                                        <h4 class="text-lg font-bold text-black mb-2 font-barlow-condensed">Smarter
                                            Workflows, Less Supervision</h4>
                                        <p class="text-gray-900 leading-relaxed">We train your team to streamline tasks,
                                            manage their time, and collaborate better, so things run smoothly without
                                            constant oversight.</p>
                                    </div>
                                </div>
                            </div>

                            <div class="bg-white rounded-xl shadow-md p-6 border-l-4 border-green-500">
                                <div class="flex items-start gap-4">
                                    <Icon name="heroicons:academic-cap"
                                        class="w-6 h-6 text-green-500 mt-1 flex-shrink-0" />
                                    <div>
                                        <h4 class="text-lg font-bold text-black mb-2 font-barlow-condensed">Stronger
                                            Skills, Greater Autonomy</h4>
                                        <p class="text-gray-900 leading-relaxed">We build your team's ability to think
                                            independently, solve problems, and communicate clearly—reducing their need
                                            for constant direction.</p>
                                    </div>
                                </div>
                            </div>

                            <div class="bg-white rounded-xl shadow-md p-6 border-l-4 border-purple-500">
                                <div class="flex items-start gap-4">
                                    <Icon name="heroicons:shield-check"
                                        class="w-6 h-6 text-purple-500 mt-1 flex-shrink-0" />
                                    <div>
                                        <h4 class="text-lg font-bold text-black mb-2 font-barlow-condensed">Ownership
                                            Culture</h4>
                                        <p class="text-gray-900 leading-relaxed">Employees thrive when trusted to
                                            deliver. We help build a culture where they take ownership, make proactive
                                            moves, and add real value.</p>
                                    </div>
                                </div>
                            </div>

                            <div class="bg-white rounded-xl shadow-md p-6 border-l-4 border-orange-500">
                                <div class="flex items-start gap-4">
                                    <Icon name="heroicons:users" class="w-6 h-6 text-orange-500 mt-1 flex-shrink-0" />
                                    <div>
                                        <h4 class="text-lg font-bold text-black mb-2 font-barlow-condensed">Better
                                            Collaboration, Superior Results</h4>
                                        <p class="text-gray-900 leading-relaxed">With improved communication and
                                            teamwork, your team works as one cohesive unit, driving better outcomes with
                                            less friction.</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Quality Pledge Section -->
            <section class="mb-24">
                <div class="text-center mb-16 mx-4 lg:mx-8">
                    <h3 class="text-3xl lg:text-4xl font-bold text-black mb-6 font-barlow-condensed">
                        The Wilson Samson Quality Pledge
                    </h3>
                    <div class="w-24 h-1 bg-blue-600 rounded-full mx-auto"></div>
                </div>

                <div class="grid md:grid-cols-3 gap-8 mx-4 lg:mx-8">
                    <div
                        class="bg-gradient-to-br from-blue-50 to-white rounded-xl shadow-md p-8 hover:shadow-lg transition-shadow duration-300 text-center border border-blue-100">
                        <div class="bg-blue-600 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-6">
                            <Icon name="heroicons:wrench-screwdriver" class="w-8 h-8 text-white" />
                        </div>
                        <h4 class="text-xl font-bold text-black mb-4 font-barlow-condensed">Custom-Fit for Your Business
                        </h4>
                        <p class="text-gray-900 leading-relaxed">We tailor every solution to your specific team,
                            operations, and goals—no generic, one-size-fits-all approaches.</p>
                    </div>

                    <div
                        class="bg-gradient-to-br from-green-50 to-white rounded-xl shadow-md p-8 hover:shadow-lg transition-shadow duration-300 text-center border border-green-100">
                        <div class="bg-green-600 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-6">
                            <Icon name="heroicons:chart-bar-square" class="w-8 h-8 text-white" />
                        </div>
                        <h4 class="text-xl font-bold text-black mb-4 font-barlow-condensed">Tangible Results</h4>
                        <p class="text-gray-900 leading-relaxed">Our proven training methods aren't theory—they're
                            tested systems that improve business efficiency and team performance.</p>
                    </div>

                    <div
                        class="bg-gradient-to-br from-purple-50 to-white rounded-xl shadow-md p-8 hover:shadow-lg transition-shadow duration-300 text-center border border-purple-100">
                        <div class="bg-purple-600 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-6">
                            <Icon name="heroicons:trophy" class="w-8 h-8 text-white" />
                        </div>
                        <h4 class="text-xl font-bold text-black mb-4 font-barlow-condensed">Long-Term Wins</h4>
                        <p class="text-gray-900 leading-relaxed">The more empowered your team becomes, the more space
                            you gain to focus on growth and big-picture strategic thinking.</p>
                    </div>
                </div>
            </section>

            <!-- Support Section -->
            <section class="mb-24">
                <div class="bg-gray-100 rounded-2xl p-8 lg:p-12 mx-4 lg:mx-8">
                    <div class="text-center mb-8">
                        <h3 class="text-2xl lg:text-3xl font-bold text-black mb-4 font-barlow-condensed">
                            Ongoing Support That Ensures Success
                        </h3>
                        <p class="text-lg text-gray-900 leading-relaxed max-w-3xl mx-auto">
                            We don't just train and disappear. We stay with you post-training—checking in,
                            offering feedback, and making sure productivity gains stick for the long term.
                        </p>
                    </div>
                    <div class="flex justify-center">
                        <div class="bg-white rounded-xl shadow-md p-6 max-w-md">
                            <div class="flex items-center gap-4 mb-4">
                                <Icon name="heroicons:phone" class="w-6 h-6 text-blue-600" />
                                <h4 class="text-lg font-bold text-black font-barlow-condensed">Follow-Up Sessions</h4>
                            </div>
                            <div class="flex items-center gap-4 mb-4">
                                <Icon name="heroicons:chat-bubble-left-right" class="w-6 h-6 text-green-600" />
                                <h4 class="text-lg font-bold text-black font-barlow-condensed">Progress Reviews</h4>
                            </div>
                            <div class="flex items-center gap-4">
                                <Icon name="heroicons:arrow-trending-up" class="w-6 h-6 text-purple-600" />
                                <h4 class="text-lg font-bold text-black font-barlow-condensed">Continuous Improvement
                                </h4>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Final CTA Section -->
            <section class="mb-16">
                <div
                    class="bg-gradient-to-r from-blue-600 to-blue-700 text-white rounded-2xl p-8 lg:p-12 mx-4 lg:mx-8 text-center">
                    <h3 class="text-3xl lg:text-4xl font-bold mb-6 font-barlow-condensed">
                        Ready to Transform Your Team and Reclaim Your Time?
                    </h3>
                    <p class="text-xl text-blue-100 mb-8 leading-relaxed max-w-3xl mx-auto">
                        Stop being the bottleneck in your own business. Empower your team to work smarter,
                        think independently, and drive results while you focus on what matters most—growing your
                        business.
                    </p>
                    <div class="flex flex-col sm:flex-row gap-4 justify-center">
                        <NuxtLink to="/contact" target="_blank"
                            class="bg-white hover:bg-gray-100 text-blue-600 px-8 py-4 rounded-lg font-semibold transition-all duration-300 text-center shadow-lg hover:shadow-xl">
                            <Icon name="heroicons:rocket-launch" class="w-5 h-5 mr-2 inline" />
                            Start Your Team Transformation
                        </NuxtLink>
                        <a href="https://wa.me/2348132924637"
                            class="border-2 border-white hover:border-blue-200 text-white hover:bg-white hover:text-blue-600 px-8 py-4 rounded-lg font-semibold transition-all duration-300 text-center">
                            <Icon name="heroicons:phone" class="w-5 h-5 mr-2 inline" />
                            Get Free Consultation
                        </a>
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

.animate-fade-in {
    animation: fadeIn 0.8s ease-out forwards;
}

/* Card hover effects */
.bg-white:hover {
    transform: translateY(-2px);
}

/* Gradient hover effects */
.bg-gradient-to-br:hover {
    transform: translateY(-4px);
}

/* Social media icons animation */
.fixed>a {
    animation: slideInLeft 0.6s ease-out forwards;
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