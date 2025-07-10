<template>
    <section class="program-details py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="max-w-4xl mx-auto">
                <div class="grid md:grid-cols-2 gap-12">
                    <div>
                        <h3 class="text-2xl font-bold text-gray-900 mb-6">What's Included:</h3>
                        <ul class="space-y-4">
                            <li v-for="item in included" :key="item" class="flex items-start">
                                <Icon name="heroicons:check" class="h-5 w-5 text-green-500 mt-1 mr-3 flex-shrink-0" />
                                <span class="text-gray-600">{{ item }}</span>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <h3 class="text-2xl font-bold text-gray-900 mb-6">What You'll Walk Away With:</h3>
                        <ul class="space-y-4">
                            <li v-for="outcome in outcomes" :key="outcome" class="flex items-start">
                                <Icon name="heroicons:check" class="h-5 w-5 text-blue-500 mt-1 mr-3 flex-shrink-0" />
                                <span class="text-gray-600">{{ outcome }}</span>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>

const included = [
    "One-on-one clarity coaching sessions with Wilson",
    "Goal-setting and vision-alignment exercises",
    "Strategy tools designed around and customized to your specific business",
    "Simple, actionable plans you can implement immediately",
    "Optional support for content planning or book strategy (if visibility is a goal)"
]

const outcomes = [
    "A clear, personal roadmap for your business",
    "More time and headspace to focus on what truly matters",
    "A self-sufficient team that doesn't need you 24/7",
    "Renewed clarity, confidence, and energy",
    "Tools to finally bring your expertise into the spotlight — via writing, speaking, or publishing"
]
</script>