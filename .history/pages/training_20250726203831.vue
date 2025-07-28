<template>
    <div class="min-h-screen bg-gray-50">
        <!-- Social Media Icons - Sticky -->
        <LandingSocialMedia />
        <!-- Main Content -->
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">

            <!-- Hero Section -->
            <section class="mb-24 pt-8 lg:pt-28">
                <div class="grid lg:grid-cols-2 gap-8 lg:gap-10 items-center">
                    <!-- Content Column -->
                    <div class="space-y-6 mx-2 sm:mx-4 lg:mx-6">
                        <h3
                            class="inline-flex items-center gap-2 bg-blue-100 text-blue-700 px-4 py-2 rounded-lg text-base font-medium">
                            <Icon name="heroicons:users" class="w-5 h-5" />
                            FROM DISENGAGED TO DRIVEN
                        </h3>
                        <h1
                            class="text-3xl sm:text-4xl lg:text-5xl font-bold text-black leading-tight font-barlow-condensed">
                            Boost Your Business with
                            <span class="text-blue-600">Employee Productivity Programs</span>
                        </h1>
                        <p class="text-base sm:text-lg text-gray-900 leading-relaxed">
                            Running a business shouldn't mean handling every task yourself. If your daily operations
                            constantly demand your attention, it's time for a shift.
                        </p>
                        <p class="text-base sm:text-lg text-gray-900 leading-relaxed">
                            Our <b>Employee Productivity Programs</b> are built to help you step back from the weeds and
                            lead
                            at a higher level, while your team becomes more capable, accountable, and productive.
                        </p>
                        <div class="flex flex-col sm:flex-row gap-4">
                            <NuxtLink to="/contact" target="_blank"
                                class="bg-gray-900 hover:bg-blue-600 text-white px-6 py-3 rounded-lg font-semibold transition-all duration-300 text-center">
                                Transform Your Team
                            </NuxtLink>
                            <a href="https://wa.me/2348132924637"
                                class="border border-gray-900 hover:bg-blue-600 text-gray-900 hover:text-white px-6 py-3 rounded-lg font-semibold transition-all duration-300 text-center">
                                Free Consultation
                            </a>
                        </div>
                    </div>

                    <!-- Image Column -->
                    <div class="relative group mx-2 sm:mx-4 lg:mx-6 mt-8 lg:mt-24">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105">
                            <img src="~/assets/img/wilsonsamson-training.jpg" alt="Employee productivity training"
                                class="w-full h-[300px] sm:h-[350px] lg:h-[400px] object-cover" />
                        </div>
                    </div>
                </div>
            </section>

            <!-- Problems & Solutions Combined -->
            <section class="mb-24">
                <div class="text-center mb-16 mx-2 sm:mx-4 lg:mx-6">
                    <h2 class="text-2xl sm:text-3xl lg:text-4xl font-bold text-black mb-6 font-barlow-condensed">
                        What You Get
                    </h2>
                    <div class="w-24 h-1 bg-blue-600 rounded-full mx-auto"></div>
                </div>

                <div class="grid lg:grid-cols-2 gap-8 lg:gap-10 items-start">
                    <!-- Benefits Column -->
                    <div class="space-y-6 mx-2 sm:mx-4 lg:mx-6">
                        <div
                            class="bg-white rounded-xl drop-shadow-lg p-4 sm:p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-3 sm:gap-4">
                                <Icon name="heroicons:cog-6-tooth"
                                    class="w-5 h-5 sm:w-6 sm:h-6 text-blue-600 mt-1 flex-shrink-0" />
                                <div>
                                    <h3 class="text-lg sm:text-xl font-bold text-black mb-2 font-barlow-condensed">
                                        Smarter
                                        Workflow, Less Supervision
                                    </h3>
                                    <p class="text-sm sm:text-base text-gray-900">We train your team to streamline
                                        tasks, manage their time,
                                        and collaborate better, so things run smoothly without you having to oversee
                                        every move.
                                    </p>
                                </div>
                            </div>
                        </div>

                        <div
                            class="bg-white rounded-xl drop-shadow-lg p-4 sm:p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-3 sm:gap-4">
                                <Icon name="heroicons:academic-cap"
                                    class="w-5 h-5 sm:w-6 sm:h-6 text-blue-600 mt-1 flex-shrink-0" />
                                <div>
                                    <h3 class="text-lg sm:text-xl font-bold text-black mb-2 font-barlow-condensed">
                                        Stronger Skills,
                                        Greater Autonomy
                                    </h3>
                                    <p class="text-sm sm:text-base text-gray-900">We build up your team's ability to
                                        think independently,
                                        solve problems, and communicate clearly. In essence, they're empowered with
                                        skills that fuel better decisions and
                                        reduce the need for constant direction.
                                    </p>
                                </div>
                            </div>
                        </div>

                        <div
                            class="bg-white rounded-xl drop-shadow-lg p-4 sm:p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-3 sm:gap-4">
                                <Icon name="heroicons:shield-check"
                                    class="w-5 h-5 sm:w-6 sm:h-6 text-blue-600 mt-1 flex-shrink-0" />
                                <div>
                                    <h3 class="text-lg sm:text-xl font-bold text-black mb-2 font-barlow-condensed">
                                        Ownership
                                        Culture</h3>
                                    <p class="text-sm sm:text-base text-gray-900">Employees thrive when they're trusted
                                        to deliver. We help
                                        you build a culture where they take ownership, make proactive moves, and bring
                                        more value to the business.</p>
                                </div>
                            </div>
                        </div>

                        <div
                            class="bg-white rounded-xl drop-shadow-lg p-4 sm:p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-3 sm:gap-4">
                                <Icon name="heroicons:hand-thumb-up"
                                    class="w-5 h-5 sm:w-6 sm:h-6 text-blue-600 mt-1 flex-shrink-0" />
                                <div>
                                    <h3 class="text-lg sm:text-xl font-bold text-black mb-2 font-barlow-condensed">
                                        Stronger
                                        Collaboration, Better Results
                                    </h3>
                                    <p class="text-sm sm:text-base text-gray-900">With improved communication and
                                        teamwork, your team works
                                        as one cohesive unit, driving better outcomes with less friction.</p>
                                </div>
                            </div>
                        </div>
                        <div
                            class="bg-white rounded-xl drop-shadow-lg p-4 sm:p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-3 sm:gap-4">
                                <Icon name="heroicons:chart-bar"
                                    class="w-5 h-5 sm:w-6 sm:h-6 text-blue-600 mt-1 flex-shrink-0" />

                                <div>
                                    <h3 class="text-lg sm:text-xl font-bold text-black mb-2 font-barlow-condensed">
                                        Ongoing Support
                                    </h3>
                                    <p class="text-sm sm:text-base text-gray-900">We stay with you post-training;
                                        checking in, offering
                                        feedback, and making sure productivity gains stick.</p>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Image Column -->
                    <div class="relative mx-2 sm:mx-4 lg:mx-6 space-y-6">
                        <div class="overflow-hidden rounded-2xl shadow-2xl">
                            <img src="~/assets/img/wilsonsamson-training2.jpg" alt="Team collaboration training"
                                class="w-full h-[180px] sm:h-[200px] lg:h-[270px] object-cover" />
                        </div>
                        <div class="overflow-hidden rounded-2xl shadow-2xl">
                            <img src="~/assets/img/wilsonsamson-training4.jpg" alt="Professional skills development"
                                class="w-full h-[180px] sm:h-[200px] lg:h-[270px] object-cover" />
                        </div>
                        <div class="overflow-hidden rounded-2xl shadow-2xl">
                            <img src="~/assets/img/wilsonsamson-training3.jpg" alt="Professional development session"
                                class="w-full h-[180px] sm:h-[200px] lg:h-[270px] object-cover" />
                        </div>
                    </div>
                </div>
            </section>

            <!-- Quality Guarantee -->
            <section class="mb-24">
                <div class="bg-gray-900 text-white rounded-2xl p-6 sm:p-8 lg:p-12 mx-2 sm:mx-4 lg:mx-6">
                    <div class="text-center mb-8">
                        <h3 class="text-xl sm:text-2xl lg:text-3xl font-bold mb-4 font-barlow-condensed">
                            The <span class="text-blue-300 glow-text">Wilson Samson</span> Quality Pledge
                        </h3>
                    </div>
                    <div class="grid sm:grid-cols-2 md:grid-cols-3 gap-6 sm:gap-8 text-center">
                        <div
                            class="bg-gray-800 rounded-xl p-4 sm:p-6 shadow-xl hover:shadow-2xl hover:scale-105 transition-all duration-300 animate-on-hover">
                            <Icon name="heroicons:wrench-screwdriver"
                                class="w-6 h-6 sm:w-8 sm:h-8 text-blue-400 mx-auto mb-4" />
                            <h4 class="text-base sm:text-lg font-bold mb-2 font-barlow-condensed">Custom-Fit Solutions
                            </h4>
                            <p class="text-sm sm:text-base text-gray-300 text-left">Every solution is designed around
                                your unique team,
                                goals, and operations. No templates. No one-size-fits-all approach.</p>
                        </div>
                        <div
                            class="bg-gray-800 rounded-xl p-4 sm:p-6 shadow-xl hover:shadow-2xl hover:scale-105 transition-all duration-300 animate-on-hover">
                            <Icon name="heroicons:chart-bar-square"
                                class="w-6 h-6 sm:w-8 sm:h-8 text-blue-400 mx-auto mb-4" />
                            <h4 class="text-base sm:text-lg font-bold mb-2 font-barlow-condensed">Proven Results</h4>
                            <p class="text-sm sm:text-base text-gray-300 text-left">Our frameworks are based on real
                                business outcomes. Plus
                                you'll see measurable improvements in how your team operates.</p>
                        </div>
                        <div
                            class="bg-gray-800 rounded-xl p-4 sm:p-6 shadow-xl hover:shadow-2xl hover:scale-105 transition-all duration-300 animate-on-hover sm:col-span-2 md:col-span-1">
                            <Icon name="heroicons:trophy" class="w-6 h-6 sm:w-8 sm:h-8 text-blue-400 mx-auto mb-4" />
                            <h4 class="text-base sm:text-lg font-bold mb-2 font-barlow-condensed">Long-Term Impact</h4>
                            <p class="text-sm sm:text-base text-gray-300 text-left">We help you build capacity in your
                                team so you can
                                finally step back and think bigger. That's how sustainable growth happens.</p>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Final CTA -->
            <section class="mb-16">
                <div class="text-center mx-2 sm:mx-4 lg:mx-6">
                    <h3 class="text-2xl sm:text-3xl lg:text-4xl font-bold text-black mb-6 font-barlow-condensed">
                        Ready to Transform Your Team?
                    </h3>
                    <p class="text-base sm:text-lg text-gray-900 mb-8 max-w-2xl mx-auto">
                        Stop being the bottleneck. Empower your team to work independently while you reclaim your
                        time and focus on growing
                        your business.
                    </p>
                    <div class="flex flex-col sm:flex-row gap-4 justify-center">
                        <NuxtLink to="/contact" target="_blank"
                            class="bg-gray-900 hover:bg-blue-600 text-white px-6 py-3 rounded-lg font-semibold transition-all duration-300 text-center">
                            Start Transformation
                        </NuxtLink>
                        <a href="https://wa.me/2348132924637"
                            class="border border-gray-900 hover:bg-blue-600 text-gray-900 hover:text-white px-6 py-3 rounded-lg font-semibold transition-all duration-300 text-center">
                            Free Consultation
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

.animate-fade-in {
    animation: fadeIn 0.8s ease-out forwards;
}

/* Card hover effects */
.bg-white:hover {
    transform: translateY(-2px);
}

/* Glow effect for text */
.glow-text {
    text-shadow: 0 0 10px rgba(147, 197, 253, 0.5);
}

/* Enhanced responsive design */
@media (max-width: 640px) {
    .mx-2 {
        margin-left: 0.5rem;
        margin-right: 0.5rem;
    }

    /* Ensure buttons stack nicely on mobile */
    .flex-col {
        align-items: stretch;
    }

    /* Optimize text sizes for mobile readability */
    .text-3xl {
        line-height: 1.2;
    }
}

@media (min-width: 640px) and (max-width: 1023px) {
    .sm\:mx-4 {
        margin-left: 1rem;
        margin-right: 1rem;
    }
}

@media (min-width: 1024px) {
    .lg\:mx-6 {
        margin-left: 1.5rem;
        margin-right: 1.5rem;
    }
}

/* Optimize image loading and performance */
img {
    image-rendering: -webkit-optimize-contrast;
    image-rendering: crisp-edges;
}

/* Smooth transitions for all interactive elements */
* {
    transition-property: color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, backdrop-filter;
    transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
    transition-duration: 150ms;
}

/* Enhanced hover effects */
.group:hover .group-hover\:scale-105 {
    transform: scale(1.02);
}

/* Improved focus states for accessibility */
a:focus,
button:focus {
    outline: 2px solid #3B82F6;
    outline-offset: 2px;
}
</style>