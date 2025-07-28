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
                            class="inline-flex items-center gap-2 bg-blue-100 text-blue-700 px-4 py-2 rounded-lg text-base font-medium">
                            <Icon name="heroicons:users" class="w-5 h-5" />
                            FROM OVERWORKED TO EMPOWERED
                        </h3>
                        <h1 class="text-4xl lg:text-5xl font-bold text-black leading-tight font-barlow-condensed">
                            Boost Your Business with
                            <span class="text-blue-600">Employee Productivity Programs</span>
                        </h1>
                        <p class="text-lg text-gray-900 leading-relaxed">
                            Running a business shouldn’t mean handling every task yourself. If your daily operations
                            constantly demand your attention, it’s time for a shift.
                        </p>
                        <p class="text-lg text-gray-900 leading-relaxed">
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
                                class="border border-gray-900 hover:bg-blue-600  text-gray-900 hover:text-white px-6 py-3 rounded-lg font-semibold transition-all duration-300 text-center">
                                Free Consultation
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
                    </div>
                </div>
            </section>

            <!-- Problems & Solutions Combined -->
            <section class="mb-24">
                <div class="text-center mb-16 mx-4 lg:mx-8">
                    <h2 class="text-3xl lg:text-4xl font-bold text-black mb-6 font-barlow-condensed">
                        What You Get
                    </h2>
                    <div class="w-24 h-1 bg-blue-600 rounded-full mx-auto"></div>
                </div>

                <div class="grid lg:grid-cols-2 gap-12 items-center">
                    <!-- Benefits Column -->
                    <div class="space-y-6 mx-4 lg:mx-8">
                        <div
                            class="bg-white rounded-xl drop-shadow-lg p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-4">
                                <Icon name="heroicons:cog-6-tooth" class="w-6 h-6 text-blue-600 mt-1 flex-shrink-0" />
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Smarter
                                        Workflow, Less Supervision
                                    </h3>
                                    <p class="text-gray-900">We train your team to streamline tasks, manage their time,
                                        and collaborate better, so things run smoothly without you having to oversee
                                        every move.
                                    </p>
                                </div>
                            </div>
                        </div>

                        <div
                            class="bg-white rounded-xl drop-shadow-lg p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-4">
                                <Icon name="heroicons:academic-cap" class="w-6 h-6 text-blue-600 mt-1 flex-shrink-0" />
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Stronger Skills,
                                        Greater Autonomy
                                    </h3>
                                    <p class="text-gray-900">We build up your team’s ability to think independently,
                                        solve problems, and communicate clearly. In essence, they're empoweted with
                                        skills that fuel better decisions and
                                        reduce the need for constant direction.
                                    </p>
                                </div>
                            </div>
                        </div>

                        <div
                            class="bg-white rounded-xl drop-shadow-lg p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-4">
                                <Icon name="heroicons:shield-check" class="w-6 h-6 text-blue-600 mt-1 flex-shrink-0" />
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Ownership
                                        Culture</h3>
                                    <p class="text-gray-900">Employees thrive when they’re trusted to deliver. We help
                                        you build a culture where they take ownership, make proactive moves, and bring
                                        more value to the business.</p>
                                </div>
                            </div>
                        </div>

                        <div
                            class="bg-white rounded-xl drop-shadow-lg p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-4">
                                <Icon name="heroicons:hand-thumb-up" class="w-6 h-6 text-blue-600 mt-1 flex-shrink-0" />
                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Stronger
                                        Collaboration, Better Results

                                    </h3>
                                    <p class="text-gray-900">With improved communication and teamwork, your team works
                                        as one cohesive unit, driving better outcomes with less friction.</p>
                                </div>
                            </div>
                        </div>
                        <div
                            class="bg-white rounded-xl drop-shadow-lg p-6 hover:shadow-lg transition-shadow duration-300">
                            <div class="flex items-start gap-4">
                                <Icon name="heroicons:chart-bar" class="w-6 h-6 text-blue-600 mt-1 flex-shrink-0" />

                                <div>
                                    <h3 class="text-xl font-bold text-black mb-2 font-barlow-condensed">Stronger
                                        Ongoing Support

                                    </h3>
                                    <p class="text-gray-900">We stay with you post-training; checking in, offering
                                        feedback, and making sure productivity gains stick.</p>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Image Column -->
                    <div class="relative group mx-4 lg:mx-8">
                        <div
                            class="overflow-hidden rounded-2xl shadow-2xl transition-transform duration-500 group-hover:scale-105">
                            <img src="~/assets/img/wilsonsamson-hero-image3.png" alt="Team collaboration"
                                class="w-full h-[500px] object-cover" />
                        </div>
                    </div>
                </div>
            </section>

            <section class="mb-16">
                <div class="bg-gray-900 text-white rounded-2xl p-8 lg:p-12 mx-4 lg:mx-8 shadow-xl">
                    <div class="text-center mb-8">
                        <h3 class="text-2xl lg:text-3xl font-bold mb-4 font-barlow-condensed">
                            The <span class="text-blue-300 glow-effect">Wilson Samson</span> Quality Pledge
                        </h3>
                    </div>
                    <div class="grid md:grid-cols-3 gap-6">
                        <div class="bg-gray-800/50 p-6 rounded-lg shadow-md hover:shadow-lg transition-shadow">
                            <Icon name="heroicons:wrench-screwdriver" class="w-8 h-8 text-blue-400 mx-auto mb-4" />
                            <h4 class="text-lg font-bold mb-2 font-barlow-condensed">Custom-Fit Solutions</h4>
                            <p class="text-gray-300">Every solution is designed around your unique team, goals, and
                                operations.</p>
                        </div>
                        <div class="bg-gray-800/50 p-6 rounded-lg shadow-md hover:shadow-lg transition-shadow">
                            <Icon name="heroicons:chart-bar-square" class="w-8 h-8 text-blue-400 mx-auto mb-4" />
                            <h4 class="text-lg font-bold mb-2 font-barlow-condensed">Proven Results</h4>
                            <p class="text-gray-300">Our frameworks deliver measurable improvements in team operations.
                            </p>
                        </div>
                        <div class="bg-gray-800/50 p-6 rounded-lg shadow-md hover:shadow-lg transition-shadow">
                            <Icon name="heroicons:trophy" class="w-8 h-8 text-blue-400 mx-auto mb-4" />
                            <h4 class="text-lg font-bold mb-2 font-barlow-condensed">Long-Term Impact</h4>
                            <p class="text-gray-300">Build team capacity so you can focus on sustainable growth.</p>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Final CTA -->
            <section class="mb-16">
                <div class="text-center mx-4 lg:mx-8">
                    <h3 class="text-3xl lg:text-4xl font-bold text-black mb-6 font-barlow-condensed">
                        Ready to Transform Your Team?
                    </h3>
                    <p class="text-lg text-gray-900 mb-8 max-w-2xl mx-auto">
                        Stop being the bottleneck. Empower your team to work independently while you reclaim your
                        time and focus on growing
                        your business.
                    </p>
                    <div class="flex flex-col sm:flex-row gap-4 justify-center">
                        <NuxtLink to="/contact" target="_blank"
                            class="bg-blue-600 hover:bg-blue-700 text-white px-8 py-4 rounded-lg font-semibold transition-all duration-300 text-center">
                            Start Transformation
                        </NuxtLink>
                        <a href="https://wa.me/2348132924637"
                            class="border border-blue-600 hover:bg-blue-600 hover:text-white px-8 py-4 rounded-lg font-semibold transition-all duration-300 text-center">
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

/* Responsive adjustments */
@media (max-width: 768px) {
    .mx-4 {
        margin-left: 1rem;
        margin-right: 1rem;
    }
}

@media (min-width: 1024px) {
    .lg\:mx-8 {
        margin-left: 2rem;
        margin-right: 2rem;
    }
}

.glow-effect {
    text-shadow: 0 0 8px rgba(147, 197, 253, 0.5);
    transition: text-shadow 0.3s ease;
}

.glow-effect:hover {
    text-shadow: 0 0 12px rgba(147, 197, 253, 0.7);
}

.shadow-md {
    box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
}

.shadow-lg {
    box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
}
</style>