<template>
    <div class="min-h-screen bg-gray-50">
        <!-- Social Media Icons - Sticky -->
        <LandingSocialMedia />

        <!-- Main Content -->
        <div class="max-w-4xl mx-auto px-4 sm:px-6 py-16">

            <!-- Hero Section -->
            <section class="mb-20 pt-8">
                <div class="grid lg:grid-cols-2 gap-8 items-center">
                    <div class="space-y-4">
                        <h3 class="text-sm font-medium text-gray-600">
                            TEAM PRODUCTIVITY SOLUTIONS
                        </h3>
                        <h1 class="text-3xl lg:text-4xl font-bold text-black font-barlow-condensed">
                            Empower Your Team, <span class="text-blue-600">Elevate Your Business</span>
                        </h1>
                        <p class="text-gray-700">
                            Transform your workforce from dependent to self-sufficient with our targeted productivity
                            programs.
                        </p>
                        <div class="flex flex-col sm:flex-row gap-3">
                            <NuxtLink to="/contact"
                                class="bg-black text-white px-5 py-2.5 rounded-lg font-medium text-center">
                                Get Started
                            </NuxtLink>
                        </div>
                    </div>

                    <div class="relative group">
                        <div class="overflow-hidden rounded-xl shadow-lg">
                            <img src="~/assets/img/burnoout-clarity.jpeg" alt="Team productivity"
                                class="w-full h-[300px] object-cover" />
                        </div>
                    </div>
                </div>
            </section>

            <!-- Core Benefits Section -->
            <section class="mb-20">
                <div class="text-center mb-10">
                    <h2 class="text-2xl font-bold text-black font-barlow-condensed">
                        What We Deliver
                    </h2>
                    <div class="w-16 h-1 bg-gray-300 rounded-full mx-auto mt-3"></div>
                </div>

                <div class="grid md:grid-cols-2 gap-6">
                    <div class="bg-white p-5 rounded-lg border border-gray-200">
                        <div class="flex items-start gap-3">
                            <Icon name="heroicons:arrow-trending-up"
                                class="w-5 h-5 text-blue-600 mt-0.5 flex-shrink-0" />
                            <div>
                                <h3 class="font-bold text-black mb-1">Streamlined Workflows</h3>
                                <p class="text-gray-700 text-sm">Reduce bottlenecks and redundant processes.</p>
                            </div>
                        </div>
                    </div>

                    <div class="bg-white p-5 rounded-lg border border-gray-200">
                        <div class="flex items-start gap-3">
                            <Icon name="heroicons:light-bulb" class="w-5 h-5 text-blue-600 mt-0.5 flex-shrink-0" />
                            <div>
                                <h3 class="font-bold text-black mb-1">Autonomous Teams</h3>
                                <p class="text-gray-700 text-sm">Develop critical thinking and decision-making skills.
                                </p>
                            </div>
                        </div>
                    </div>

                    <div class="bg-white p-5 rounded-lg border border-gray-200">
                        <div class="flex items-start gap-3">
                            <Icon name="heroicons:hand-raised" class="w-5 h-5 text-blue-600 mt-0.5 flex-shrink-0" />
                            <div>
                                <h3 class="font-bold text-black mb-1">Ownership Culture</h3>
                                <p class="text-gray-700 text-sm">Team members take initiative and responsibility.</p>
                            </div>
                        </div>
                    </div>

                    <div class="bg-white p-5 rounded-lg border border-gray-200">
                        <div class="flex items-start gap-3">
                            <Icon name="heroicons:users" class="w-5 h-5 text-blue-600 mt-0.5 flex-shrink-0" />
                            <div>
                                <h3 class="font-bold text-black mb-1">Better Collaboration</h3>
                                <p class="text-gray-700 text-sm">Clear communication and aligned goals.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- How It Works Section -->
            <section class="mb-20 bg-white rounded-xl p-8 shadow-sm">
                <div class="text-center mb-8">
                    <h2 class="text-2xl font-bold text-black font-barlow-condensed">
                        Simple Implementation
                    </h2>
                    <div class="w-16 h-1 bg-gray-300 rounded-full mx-auto mt-3"></div>
                </div>

                <div class="space-y-8">
                    <div class="flex gap-4">
                        <div
                            class="bg-gray-800 text-white w-8 h-8 rounded-full flex items-center justify-center flex-shrink-0 mt-0.5">
                            1
                        </div>
                        <div>
                            <h3 class="font-bold text-black">Assessment</h3>
                            <p class="text-gray-700 text-sm">We analyze your team's current productivity gaps.</p>
                        </div>
                    </div>

                    <div class="flex gap-4">
                        <div
                            class="bg-gray-800 text-white w-8 h-8 rounded-full flex items-center justify-center flex-shrink-0 mt-0.5">
                            2
                        </div>
                        <div>
                            <h3 class="font-bold text-black">Targeted Training</h3>
                            <p class="text-gray-700 text-sm">Customized sessions addressing your specific needs.</p>
                        </div>
                    </div>

                    <div class="flex gap-4">
                        <div
                            class="bg-gray-800 text-white w-8 h-8 rounded-full flex items-center justify-center flex-shrink-0 mt-0.5">
                            3
                        </div>
                        <div>
                            <h3 class="font-bold text-black">Sustainable Results</h3>
                            <p class="text-gray-700 text-sm">Ongoing support to ensure lasting improvements.</p>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Final CTA -->
            <section class="text-center">
                <div class="bg-gray-900 text-white rounded-xl p-8">
                    <h3 class="text-xl font-bold font-barlow-condensed mb-4">Ready to transform your team?</h3>
                    <p class="text-gray-300 mb-6 text-sm">Let's discuss how we can boost your team's productivity.</p>
                    <NuxtLink to="/contact" class="inline-block bg-white text-black px-6 py-2.5 rounded-lg font-medium">
                        Start Now
                    </NuxtLink>
                </div>
            </section>

        </div>
    </div>
</template>

<script setup>
definePageMeta({
    layout: "landing"
})
</script>

<style scoped>
/* Simple hover effects */
.bg-white:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
}
</style>