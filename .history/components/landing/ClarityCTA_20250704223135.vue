<template>
    <section id="contact" class="py-20 bg-gray-900 text-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-3xl md:text-4xl font-bold mb-6">
                Tired of the Burnout Loop?
            </h2>
            <h3 class="text-xl md:text-2xl font-semibold mb-8 text-gray-300">
                Ready to Work With More Clarity and Less Pressure?
            </h3>

            <div class="bg-gray-800 rounded-2xl p-8 mb-8">
                <h4 class="text-2xl font-bold text-yellow-400 mb-4">Take the First Step</h4>
                <p class="text-lg text-gray-300 mb-8 max-w-2xl mx-auto">
                    It starts with one conversation. Find clarity, reclaim your time, and lead with ease.
                    Let's help you lead with purpose, not overwhelm.
                </p>

                <div class="flex flex-col sm:flex-row gap-4 justify-center">
                    <NuxtLink to="/book-clarity-session"
                        class="inline-flex items-center px-8 py-4 bg-yellow-400 text-gray-900 font-semibold rounded-lg hover:bg-yellow-300 transition-colors">
                        <Icon name="heroicons:calendar" class="mr-2 w-5 h-5" />
                        Book a Clarity Session
                    </NuxtLink>
                    <NuxtLink to="/discovery-call"
                        class="inline-flex items-center px-8 py-4 border-2 border-yellow-400 text-yellow-400 font-semibold rounded-lg hover:bg-yellow-400 hover:text-gray-900 transition-colors">
                        <Icon name="heroicons:phone" class="mr-2 w-5 h-5" />
                        Schedule a Discovery Call
                    </NuxtLink>
                </div>
            </div>

            <!-- Additional Contact Options -->
            <div class="grid md:grid-cols-3 gap-6 text-center">
                <div class="bg-gray-800 rounded-lg p-6">
                    <Icon name="heroicons:envelope" class="w-8 h-8 text-yellow-400 mx-auto mb-3" />
                    <h5 class="font-semibold mb-2">Email</h5>
                    <p class="text-sm text-gray-400">Get in touch directly</p>
                </div>
                <div class="bg-gray-800 rounded-lg p-6">
                    <Icon name="heroicons:phone" class="w-8 h-8 text-yellow-400 mx-auto mb-3" />
                    <h5 class="font-semibold mb-2">Phone</h5>
                    <p class="text-sm text-gray-400">Quick consultation</p>
                </div>
                <div class="bg-gray-800 rounded-lg p-6">
                    <Icon name="heroicons:calendar-days" class="w-8 h-8 text-yellow-400 mx-auto mb-3" />
                    <h5 class="font-semibold mb-2">Calendar</h5>
                    <p class="text-sm text-gray-400">Book instantly</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
// Component logic if needed
</script>