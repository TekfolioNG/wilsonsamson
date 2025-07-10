<template>
    <section class="how-it-works py-16 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="max-w-4xl mx-auto">
                <h2 class="text-3xl font-bold text-gray-900 mb-12 text-center">How It Works</h2>
                <div class="grid md:grid-cols-3 gap-8">
                    <div v-for="(step, index) in steps" :key="step.title" class="step-card text-center">
                        <div
                            class="step-number bg-blue-600 text-white rounded-full w-12 h-12 flex items-center justify-center text-xl font-bold mx-auto mb-4">
                            {{ index + 1 }}
                        </div>
                        <h3 class="text-xl font-semibold text-gray-900 mb-4">{{ step.title }}</h3>
                        <p class="text-gray-600">{{ step.description }}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
const steps = [
    {
        title: "Book a Discovery Call",
        description: "We'll identify your current challenges and what success looks like for you."
    },
    {
        title: "Schedule Your Sessions",
        description: "You'll be guided through 2–3 focused clarity sessions, with practical next steps after each."
    },
    {
        title: "Implement With Support",
        description: "You'll leave with a plan — not just ideas — and get support to follow through if needed."
    }
]
</script>
