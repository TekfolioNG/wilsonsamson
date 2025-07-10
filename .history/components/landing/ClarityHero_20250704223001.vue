<template>
    <section class="relative bg-gradient-to-br from-blue-900 to-indigo-800 text-white">
        <div class="absolute inset-0 bg-black/20"></div>
        <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-20 lg:py-32">
            <div class="lg:grid lg:grid-cols-12 lg:gap-8 items-center">
                <div class="lg:col-span-7">
                    <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-6">
                        Afraid You Could Be <span class="text-yellow-400">Burning Out?</span>
                    </h1>
                    <h2 class="text-xl md:text-2xl lg:text-3xl font-semibold mb-8 text-blue-100">
                        Do Less, Achieve More as a Business Owner or C-Suite Exec
                    </h2>
                    <p class="text-lg md:text-xl mb-8 text-blue-50 leading-relaxed">
                        Running a business shouldn't feel like a constant uphill climb. Yet many entrepreneurs and
                        professionals find themselves buried in day-to-day operations, with little room left for
                        strategy, growth, or rest.
                    </p>
                    <div class="bg-blue-800/50 backdrop-blur-sm rounded-lg p-6 mb-8">
                        <p class="text-lg font-medium text-yellow-300 mb-2">Sounds familiar?</p>
                        <p class="text-blue-100">
                            If you're overwhelmed, unclear about your direction, or simply tired of doing it all,
                            our 1-on-1 Clarity and Growth Program is built to help you reset and lead differently.
                        </p>
                    </div>
                    <div class="flex flex-col sm:flex-row gap-4">
                        <NuxtLink to="#program"
                            class="inline-flex items-center px-8 py-4 bg-yellow-400 text-blue-900 font-semibold rounded-lg hover:bg-yellow-300 transition-colors">
                            <Icon name="heroicons:arrow-right" class="ml-2 w-5 h-5" />
                            Learn More
                        </NuxtLink>
                        <NuxtLink to="#contact"
                            class="inline-flex items-center px-8 py-4 border-2 border-white text-white font-semibold rounded-lg hover:bg-white hover:text-blue-900 transition-colors">
                            <Icon name="heroicons:phone" class="mr-2 w-5 h-5" />
                            Book Discovery Call
                        </NuxtLink>
                    </div>
                </div>
                <div class="lg:col-span-5 mt-12 lg:mt-0">
                    <!-- Hero Image Placeholder -->
                    <div class="relative">
                        <div
                            class="w-full h-96 bg-gradient-to-br from-blue-600 to-purple-600 rounded-2xl flex items-center justify-center">
                            <div class="text-center">
                                <Icon name="heroicons:user-circle" class="w-32 h-32 text-white/50 mx-auto mb-4" />
                                <p class="text-white/70 text-sm">Professional Portrait</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
// Component logic if needed
</script>