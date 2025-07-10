<template>
    <section class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">
                    Are These Patterns Showing Up in Your Workflow?
                </h2>
                <p class="text-lg text-gray-600 max-w-2xl mx-auto">
                    Recognize these common challenges that keep business leaders stuck in operational mode
                </p>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
                <div v-for="problem in problems" :key="problem.id"
                    class="bg-gray-50 rounded-xl p-8 hover:shadow-lg transition-shadow">
                    <div class="w-16 h-16 bg-red-100 rounded-full flex items-center justify-center mb-6">
                        <Icon :name="problem.icon" class="w-8 h-8 text-red-600" />
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-4">
                        {{ problem.title }}
                    </h3>
                    <p class="text-gray-600 leading-relaxed">
                        {{ problem.description }}
                    </p>
                </div>
            </div>

            <div class="mt-16 text-center">
                <div class="bg-gradient-to-r from-blue-600 to-purple-600 rounded-2xl p-8 text-white">
                    <h3 class="text-2xl md:text-3xl font-bold mb-4">
                        From Burnout to Better Business
                    </h3>
                    <p class="text-xl text-blue-100 mb-6">
                        Let's Reset Your Focus with Our Proven 1-on-1 Clarity Sessions
                    </p>
                    <NuxtLink to="#program"
                        class="inline-flex items-center px-8 py-4 bg-yellow-400 text-blue-900 font-semibold rounded-lg hover:bg-yellow-300 transition-colors">
                        <Icon name="heroicons:arrow-down" class="mr-2 w-5 h-5" />
                        Discover the Solution
                    </NuxtLink>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
const problems = [
    {
        id: 1,
        title: 'Lack of Direction and Focus',
        description: "You've got ideas, but they're scattered. You want growth, but aren't sure what to prioritize.",
        icon: 'heroicons:question-mark-circle'
    },
    {
        id: 2,
        title: 'Too Much in the Weeds',
        description: "You're still making every little decision. There's no space left to breathe, let alone think long-term.",
        icon: 'heroicons:clock'
    },
    {
        id: 3,
        title: 'Team Productivity Gaps',
        description: 'Your staff depends too heavily on you. Without you in the room, things stall.',
        icon: 'heroicons:users'
    },
    {
        id: 4,
        title: 'Unexpressed Thought Leadership',
        description: "You've got valuable insights, but no time (or plan) to share them through content, books, or speaking.",
        icon: 'heroicons:light-bulb'
    }
]
</script>