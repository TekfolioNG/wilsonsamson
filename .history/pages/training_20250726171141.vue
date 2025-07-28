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
                            <Icon name="mdi:account-group" class="w-5 h-5" />
                            TEAM PRODUCTIVITY SOLUTIONS
                        </h3>
                        <h1 class="text-4xl lg:text-5xl font-bold text-black leading-tight font-barlow-condensed">
                            From Overworked to <span class="text-blue-600">Empowered</span>
                        </h1>
                        <p class="text-lg text-gray-900 leading-relaxed">
                            Running a business shouldn't mean handling every task yourself. If daily operations
                            constantly demand your attention, it's time for a shift toward sustainable productivity.
                        </p>
                        <div class="flex flex-col sm:flex-row gap-4">
                            <NuxtLink to="/contact" target="_blank"
                                class="bg-black hover:bg-white border border-gray-500 hover:border-gray-600 text-white hover:text-gray-800 px-6 py-3 rounded-lg font-semibold transition-all duration-300 text-center">
                                Explore Programs
                            </NuxtLink>
                            <a href="https://wa.me/2348132924637"
                                class="border border-gray-600 hover:border-gray-500 text-gray-800 hover:bg-black hover:text-white px-6 py-3 rounded-lg font-semibold transition-all duration-300 text-center">
                                Team Assessment
                            </a>
                        </div>
                    </div>

                    <!-- Image Column -->
                    <div class="relative group">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105 mx-4 lg:mx-8">
                            <img src="~/assets/img/burnoout-clarity.jpeg" alt="Team productivity and empowerment"
                                class="w-full h-[400px] object-cover" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300 mx-4 lg:mx-8">
                        </div>
                    </div>
                </div>
            </section>

            <!-- Value Proposition Section -->
            <section class="mb-24">
                <div class="text-center mb-16 mx-4 lg:mx-8">
                    <h2 class="text-3xl lg:text-4xl font-bold text-black mb-6 font-barlow-condensed">
                        Transform Your Team's Output
                    </h2>
                    <p class="text-xl text-gray-700 max-w-3xl mx-auto">
                        Our Employee Productivity Programs help you step back from daily operations while your team
                        becomes more capable, accountable, and productive.
                    </p>
                    <div class="w-24 h-1 bg-gray-800 rounded-full mx-auto mt-6"></div>
                </div>

                <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-start">
                    <!-- Left Column - Benefits -->
                    <div class="space-y-6 mx-4 lg:mx-8 order-1">
                        <div class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-4">
                                <div class="flex-shrink-0 mt-1">
                                    <Icon name="heroicons:arrow-trending-up" class="w-6 h-6 text-blue-600" />
                                </div>
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Smarter
                                        Workflow, Less Supervision</h3>
                                    <p class="text-gray-900 leading-relaxed">We train your team to streamline tasks,
                                        manage time effectively, and collaborate better—reducing your need to oversee
                                        every move.</p>
                                </div>
                            </div>
                        </div>

                        <div class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-4">
                                <div class="flex-shrink-0 mt-1">
                                    <Icon name="heroicons:light-bulb" class="w-6 h-6 text-blue-600" />
                                </div>
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Stronger Skills,
                                        Greater Autonomy</h3>
                                    <p class="text-gray-900 leading-relaxed">We build critical thinking,
                                        problem-solving, and communication skills that fuel better decisions and reduce
                                        constant direction.</p>
                                </div>
                            </div>
                        </div>

                        <div class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-4">
                                <div class="flex-shrink-0 mt-1">
                                    <Icon name="heroicons:hand-raised" class="w-6 h-6 text-blue-600" />
                                </div>
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Ownership
                                        Culture</h3>
                                    <p class="text-gray-900 leading-relaxed">Employees thrive when trusted. We help
                                        build a culture where team members take initiative and bring more value to the
                                        business.</p>
                                </div>
                            </div>
                        </div>

                        <div class="bg-white rounded-xl shadow-md p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-4">
                                <div class="flex-shrink-0 mt-1">
                                    <Icon name="heroicons:users" class="w-6 h-6 text-blue-600" />
                                </div>
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Stronger
                                        Collaboration</h3>
                                    <p class="text-gray-900 leading-relaxed">Improved communication and teamwork help
                                        your staff work as a cohesive unit, driving better outcomes with less friction.
                                    </p>
                                </div>
                            </div>
                        </div>

                        <!-- CTA Card -->
                        <div class="bg-gray-900 rounded-2xl p-8 mt-8">
                            <div class="space-y-6 text-gray-50">
                                <h3 class="text-2xl font-bold text-white font-barlow-condensed">Need More From Your
                                    Team?</h3>
                                <p class="text-base leading-relaxed">
                                    If you're tired of being the bottleneck in your business, our productivity programs
                                    can help your team operate at a higher level.
                                </p>
                                <NuxtLink to="/contact" target="_blank"
                                    class="w-full bg-white hover:bg-gray-100 text-black px-6 py-3 rounded-lg font-semibold transition-all duration-300 text-center block">
                                    Assess Your Team
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

            <!-- Methodology Section -->
            <section class="mb-24">
                <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-center">
                    <!-- Image Column -->
                    <div class="relative group order-2 lg:order-1">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105 mx-4 lg:mx-8">
                            <img src="~/assets/img/clarity-sessions.png" alt="Team training session"
                                class="w-full h-[400px] sm:h-[500px] lg:h-[600px] object-cover" />
                        </div>
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent rounded-2xl opacity-0 group-hover:opacity-100 transition-opacity duration-300 mx-4 lg:mx-8">
                        </div>
                    </div>

                    <!-- Content Column -->
                    <div class="space-y-8 mx-4 lg:mx-8 text-center lg:text-left order-1 lg:order-2">
                        <h3 class="text-3xl font-bold text-black font-barlow-condensed">
                            The Wilson Samson Productivity Framework
                        </h3>

                        <div class="bg-white rounded-xl shadow-md p-6 border-l-4 border-blue-600">
                            <p class="text-gray-900 leading-relaxed">
                                Our programs aren't generic training sessions. They're tailored interventions that
                                address your specific team dynamics and business needs for measurable improvement.
                            </p>
                        </div>

                        <div class="space-y-4">
                            <h4 class="text-xl font-bold text-black font-barlow-condensed">Our Approach:</h4>
                            <div class="space-y-3">
                                <div class="flex items-start">
                                    <Icon name="heroicons:magnifying-glass"
                                        class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" />
                                    <span class="text-gray-900 leading-relaxed">Comprehensive team productivity
                                        assessment</span>
                                </div>
                                <div class="flex items-start">
                                    <Icon name="heroicons:adjustments-vertical"
                                        class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" />
                                    <span class="text-gray-900 leading-relaxed">Customized training modules for your
                                        workflow</span>
                                </div>
                                <div class="flex items-start">
                                    <Icon name="heroicons:arrow-path"
                                        class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" />
                                    <span class="text-gray-900 leading-relaxed">Process optimization for recurring
                                        tasks</span>
                                </div>
                                <div class="flex items-start">
                                    <Icon name="heroicons:check-badge"
                                        class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" />
                                    <span class="text-gray-900 leading-relaxed">Accountability systems
                                        implementation</span>
                                </div>
                                <div class="flex items-start">
                                    <Icon name="heroicons:chart-bar"
                                        class="w-5 h-5 text-blue-600 mt-1 mr-3 flex-shrink-0" />
                                    <span class="text-gray-900 leading-relaxed">Performance tracking and
                                        follow-up</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Program Structure Section -->
            <section class="mb-24">
                <div class="text-center mb-16 mx-4 lg:mx-8">
                    <h3 class="text-3xl lg:text-4xl font-bold text-black mb-6 font-barlow-condensed">
                        Program Structure
                    </h3>
                    <div class="w-24 h-1 bg-gray-800 rounded-full mx-auto"></div>
                </div>

                <div class="grid md:grid-cols-3 gap-8 mx-4 lg:mx-8">
                    <div
                        class="bg-white rounded-xl shadow-md p-8 hover:shadow-lg transition-shadow duration-300 text-center">
                        <div class="bg-gray-800 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-6">
                            <Icon name="heroicons:clipboard-document-list" class="w-8 h-8 text-white" />
                        </div>
                        <h4 class="text-xl font-bold text-black mb-4 font-barlow-condensed">Assessment Phase</h4>
                        <p class="text-gray-900 leading-relaxed">We analyze your current team dynamics, workflow
                            bottlenecks, and productivity gaps.</p>
                    </div>

                    <div
                        class="bg-white rounded-xl shadow-md p-8 hover:shadow-lg transition-shadow duration-300 text-center">
                        <div class="bg-gray-800 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-6">
                            <Icon name="heroicons:academic-cap" class="w-8 h-8 text-white" />
                        </div>
                        <h4 class="text-xl font-bold text-black mb-4 font-barlow-condensed">Training Phase</h4>
                        <p class="text-gray-900 leading-relaxed">Interactive sessions focused on skill-building, process
                            improvement, and accountability.</p>
                    </div>

                    <div
                        class="bg-white rounded-xl shadow-md p-8 hover:shadow-lg transition-shadow duration-300 text-center">
                        <div class="bg-gray-800 w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-6">
                            <Icon name="heroicons:rocket-launch" class="w-8 h-8 text-white" />
                        </div>
                        <h4 class="text-xl font-bold text-black mb-4 font-barlow-condensed">Implementation</h4>
                        <p class="text-gray-900 leading-relaxed">We support your team as they apply new systems, with
                            follow-ups to ensure lasting change.</p>
                    </div>
                </div>
            </section>

            <!-- Testimonial & CTA Section -->
            <section class="mb-16">
                <div class="grid lg:grid-cols-2 gap-12 lg:gap-16 items-center">
                    <!-- Testimonial -->
                    <div class="space-y-8 mx-4 lg:mx-8">
                        <h3 class="text-3xl font-bold text-black font-barlow-condensed">
                            Client Results
                        </h3>
                        <div class="bg-white rounded-xl shadow-md p-6 border-l-4 border-blue-600">
                            <blockquote class="text-lg text-gray-900 italic mb-4 leading-relaxed">
                                "After implementing Wilson's productivity framework, our team's output increased by 40%
                                within three months. More importantly, I finally have the mental space to focus on
                                business growth instead of daily operations."
                            </blockquote>
                            <div class="font-semibold text-gray-900">— Tolu A., Manufacturing CEO</div>
                        </div>
                    </div>

                    <!-- CTA Card -->
                    <div class="bg-gray-900 text-white rounded-2xl p-8 mx-4 lg:mx-8">
                        <h4 class="text-2xl font-bold mb-6 font-barlow-condensed">Ready to Empower Your Team?</h4>
                        <p class="text-gray-300 mb-8 leading-relaxed">
                            Transform your workforce from dependent to self-sufficient with our proven productivity
                            programs.
                        </p>
                        <div class="space-y-4">
                            <NuxtLink to="/contact" target="_blank"
                                class="w-full bg-white hover:bg-gray-100 text-black px-6 py-3 rounded-lg font-semibold transition-all duration-300 flex items-center justify-center">
                                <Icon name="heroicons:envelope" class="w-5 h-5 mr-2" />
                                <span>Get Program Details</span>
                            </NuxtLink>
                            <a href="https://wa.me/2348132924637"
                                class="w-full border-2 border-gray-300 hover:border-gray-200 text-gray-300 hover:text-white px-6 py-3 rounded-lg font-semibold transition-all duration-300 flex items-center justify-center">
                                <Icon name="heroicons:phone" class="w-5 h-5 mr-2" />
                                <span>Discuss Team Needs</span>
                            </a>
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