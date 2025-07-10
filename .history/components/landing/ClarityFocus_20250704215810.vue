<template>
    <section class="problem-section py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="max-w-4xl mx-auto">
                <h2 class="text-3xl font-bold text-gray-900 mb-12 text-center">
                    Are These Patterns Showing Up in Your Workflow?
                </h2>
                <div class="grid md:grid-cols-2 gap-8">
                    <div v-for="problem in problems" :key="problem.title"
                        class="problem-card bg-gray-50 p-6 rounded-lg">
                        <h3 class="text-xl font-semibold text-gray-900 mb-4">
                            {{ problem.title }}
                        </h3>
                        <p class="text-gray-600">
                            {{ problem.description }}
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
const problems = [
    {
        title: "Lack of Direction and Focus",
        description: "You've got ideas, but they're scattered. You want growth, but aren't sure what to prioritize."
    },
    {
        title: "Too Much in the Weeds",
        description: "You're still making every little decision. There's no space left to breathe, let alone think long-term."
    },
    {
        title: "Team Productivity Gaps",
        description: "Your staff depends too heavily on you. Without you in the room, things stall."
    },
    {
        title: "Unexpressed Thought Leadership",
        description: "You've got valuable insights, but no time (or plan) to share them through content, books, or speaking."
    }
]
</script>