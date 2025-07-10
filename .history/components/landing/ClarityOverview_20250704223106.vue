<template>
    <section id="program" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <!-- Program Introduction -->
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-6">
                    The Clarity & Growth Accelerator Program
                </h2>
                <p class="text-lg text-gray-600 max-w-3xl mx-auto">
                    This is not another business seminar. It's a personalized, result-driven engagement
                    that helps you step back, regain focus, and build a real plan that aligns with your goals.
                </p>
            </div>

            <div class="grid lg:grid-cols-2 gap-16 mb-16">
                <!-- What's Included -->
                <div class="bg-white rounded-2xl p-8 shadow-lg">
                    <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mb-6">
                        <Icon name="heroicons:gift" class="w-8 h-8 text-blue-600" />
                    </div>
                    <h3 class="text-2xl font-bold text-gray-900 mb-6">What's Included</h3>
                    <ul class="space-y-4">
                        <li v-for="item in includedItems" :key="item" class="flex items-start">
                            <Icon name="heroicons:check-circle"
                                class="w-6 h-6 text-green-500 mr-3 mt-0.5 flex-shrink-0" />
                            <span class="text-gray-700">{{ item }}</span>
                        </li>
                    </ul>
                </div>

                <!-- What You'll Walk Away With -->
                <div class="bg-white rounded-2xl p-8 shadow-lg">
                    <div class="w-16 h-16 bg-green-100 rounded-full flex items-center justify-center mb-6">
                        <Icon name="heroicons:trophy" class="w-8 h-8 text-green-600" />
                    </div>
                    <h3 class="text-2xl font-bold text-gray-900 mb-6">What You'll Walk Away With</h3>
                    <ul class="space-y-4">
                        <li v-for="outcome in outcomes" :key="outcome" class="flex items-start">
                            <Icon name="heroicons:arrow-right"
                                class="w-6 h-6 text-blue-500 mr-3 mt-0.5 flex-shrink-0" />
                            <span class="text-gray-700">{{ outcome }}</span>
                        </li>
                    </ul>
                </div>
            </div>

            <!-- How It Works -->
            <div class="bg-white rounded-2xl p-8 mb-16 shadow-lg">
                <h3 class="text-2xl font-bold text-gray-900 mb-8 text-center">How It Works</h3>
                <div class="grid md:grid-cols-3 gap-8">
                    <div v-for="(step, index) in steps" :key="step.title" class="text-center">
                        <div
                            class="w-16 h-16 bg-blue-600 text-white rounded-full flex items-center justify-center mx-auto mb-4 text-2xl font-bold">
                            {{ index + 1 }}
                        </div>
                        <h4 class="text-xl font-semibold text-gray-900 mb-3">{{ step.title }}</h4>
                        <p class="text-gray-600">{{ step.description }}</p>
                    </div>
                </div>
            </div>

            <!-- Client Success Story -->
            <div class="bg-gradient-to-r from-blue-600 to-purple-600 rounded-2xl p-8 text-white">
                <div class="text-center mb-6">
                    <h3 class="text-2xl font-bold mb-4">Client Success Story</h3>
                    <div class="w-20 h-20 bg-white/20 rounded-full flex items-center justify-center mx-auto mb-4">
                        <Icon name="heroicons:chat-bubble-left-right" class="w-10 h-10 text-white" />
                    </div>
                </div>
                <blockquote class="text-lg md:text-xl italic text-center mb-6 text-blue-100">
                    "Wilson helped me reconnect with my business vision. I was stuck in the daily grind for years,
                    but after our clarity sessions, I finally had a clear direction — and the confidence to move
                    forward."
                </blockquote>
                <p class="text-center text-yellow-300 font-semibold">— Adewale B., Business Consultant</p>
            </div>
        </div>
    </section>
</template>

<script setup>
const includedItems = [
    'One-on-one clarity coaching sessions with Wilson',
    'Goal-setting and vision-alignment exercises',
    'Strategy tools designed around and customized to your specific business',
    'Simple, actionable plans you can implement immediately',
    'Optional support for content planning or book strategy (if visibility is a goal)'
]

const outcomes = [
    'A clear, personal roadmap for your business',
    'More time and headspace to focus on what truly matters',
    'A self-sufficient team that doesn\'t need you 24/7',
    'Renewed clarity, confidence, and energy',
    'Tools to finally bring your expertise into the spotlight — via writing, speaking, or publishing'
]

const steps = [
    {
        title: 'Book a Discovery Call',
        description: 'We\'ll identify your current challenges and what success looks like for you.'
    },
    {
        title: 'Schedule Your Sessions',
        description: 'You\'ll be guided through 2–3 focused clarity sessions, with practical next steps after each.'
    },
    {
        title: 'Implement With Support',
        description: 'You\'ll leave with a plan — not just ideas — and get support to follow through if needed.'
    }
]
</script>