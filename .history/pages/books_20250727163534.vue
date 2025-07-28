<template>
    <div class="min-h-screen bg-gray-50">
        <!-- Social Media Icons -->
        <LandingSocialMedia />

        <!-- Main Content -->
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
            <!-- Book Showcase Section -->
            <section class="mb-24">
                <div class="text-center mb-12">
                    <h1 class="text-3xl lg:text-4xl font-bold text-black font-barlow-condensed mb-4">
                        Books by Wilson Samson
                    </h1>
                    <div class="w-24 h-1 bg-gray-800 rounded-full mx-auto"></div>
                </div>

                <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
                    <div v-for="book in books" :key="book.title" class="group">
                        <div
                            class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition-shadow duration-300">
                            <div class="aspect-[2/3] overflow-hidden">
                                <img :src="book.image" :alt="book.title"
                                    class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                            </div>
                            <div class="p-4">
                                <h3 class="font-bold text-lg mb-2 font-barlow-condensed">{{ book.title }}</h3>
                                <a :href="book.link" target="_blank"
                                    class="inline-block bg-black text-white px-4 py-2 rounded text-sm font-medium hover:bg-gray-800 transition-colors">
                                    Get the Book
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Publishing Services Section -->
            <section class="mb-24">
                <div class="grid lg:grid-cols-2 gap-12 items-center">
                    <!-- Content Column -->
                    <div class="space-y-6">
                        <h2 class="text-3xl lg:text-4xl font-bold text-black font-barlow-condensed">
                            Be Seen. Be Trusted. Be Read.
                        </h2>
                        <h3 class="text-xl text-gray-700 font-medium">
                            Authority Positioning Through Book Publishing & Ghostwriting
                        </h3>
                        <p class="text-gray-700">
                            Your story can do more for your business than any sales pitch ever could. But writing a book
                            while running a business? We make it easy.
                        </p>
                    </div>

                    <!-- Image Column -->
                    <div class="relative group">
                        <div class="overflow-hidden rounded-xl shadow-lg">
                            <img src="~/assets/img/what-to-do-when-everything-goes-bad-wilson-samson.jpg"
                                alt="Publishing services" class="w-full h-[400px] object-cover">
                        </div>
                    </div>
                </div>
            </section>

            <!-- Services Breakdown -->
            <section class="mb-24">
                <div class="grid md:grid-cols-2 gap-8">
                    <div class="bg-white p-8 rounded-xl shadow-sm">
                        <div class="flex items-center gap-4 mb-4">
                            <div class="bg-blue-100 p-3 rounded-full">
                                <Icon name="heroicons:pencil-square" class="w-6 h-6 text-blue-600" />
                            </div>
                            <h3 class="text-xl font-bold font-barlow-condensed">We Craft Your Positioning</h3>
                        </div>
                        <p class="text-gray-700">
                            You bring the expertise; we'll help package it into a compelling narrative that positions
                            you as a trusted voice.
                        </p>
                    </div>

                    <div class="bg-white p-8 rounded-xl shadow-sm">
                        <div class="flex items-center gap-4 mb-4">
                            <div class="bg-blue-100 p-3 rounded-full">
                                <Icon name="heroicons:book-open" class="w-6 h-6 text-blue-600" />
                            </div>
                            <h3 class="text-xl font-bold font-barlow-condensed">We Do the Writing</h3>
                        </div>
                        <p class="text-gray-700">
                            From ghostwriting to content planning, we create work that builds influence without your
                            time investment.
                        </p>
                    </div>

                    <div class="bg-white p-8 rounded-xl shadow-sm">
                        <div class="flex items-center gap-4 mb-4">
                            <div class="bg-blue-100 p-3 rounded-full">
                                <Icon name="heroicons:printer" class="w-6 h-6 text-blue-600" />
                            </div>
                            <h3 class="text-xl font-bold font-barlow-condensed">We Publish You Like a Pro</h3>
                        </div>
                        <p class="text-gray-700">
                            Editing, design, printing - we handle everything. Get books delivered to your door, ready
                            for clients and events.
                        </p>
                    </div>

                    <div class="bg-white p-8 rounded-xl shadow-sm">
                        <div class="flex items-center gap-4 mb-4">
                            <div class="bg-blue-100 p-3 rounded-full">
                                <Icon name="heroicons:eye" class="w-6 h-6 text-blue-600" />
                            </div>
                            <h3 class="text-xl font-bold font-barlow-condensed">Visibility Without Burnout</h3>
                        </div>
                        <p class="text-gray-700">
                            Open doors to new opportunities while staying focused on your business.
                        </p>
                    </div>
                </div>
            </section>

            <!-- Why Choose Us -->
            <section class="mb-16 bg-gray-900 text-white rounded-2xl p-12 text-center">
                <h2 class="text-2xl lg:text-3xl font-bold mb-8 font-barlow-condensed">
                    Why Work With Us?
                </h2>
                <div class="grid md:grid-cols-3 gap-8 max-w-5xl mx-auto">
                    <div>
                        <Icon name="heroicons:clock" class="w-10 h-10 text-blue-400 mx-auto mb-4" />
                        <h3 class="text-lg font-bold mb-2 font-barlow-condensed">Minimal Time</h3>
                        <p class="text-gray-300">Stay in control without getting buried in details</p>
                    </div>
                    <div>
                        <Icon name="heroicons:megaphone" class="w-10 h-10 text-blue-400 mx-auto mb-4" />
                        <h3 class="text-lg font-bold mb-2 font-barlow-condensed">Your Voice</h3>
                        <p class="text-gray-300">Content reflects your unique tone and brand</p>
                    </div>
                    <div>
                        <Icon name="heroicons:check-badge" class="w-10 h-10 text-blue-400 mx-auto mb-4" />
                        <h3 class="text-lg font-bold mb-2 font-barlow-condensed">Proven Process</h3>
                        <p class="text-gray-300">We've helped leaders get published and noticed</p>
                    </div>
                </div>
            </section>

            <!-- Final CTA -->
            <section class="text-center">
                <h2 class="text-2xl lg:text-3xl font-bold mb-6 font-barlow-condensed">
                    Ready to become a published industry voice?
                </h2>
                <p class="text-xl text-gray-700 mb-8 max-w-3xl mx-auto">
                    Let's build your credibility while you build your business.
                </p>
                <NuxtLink to="/contact"
                    class="inline-block bg-black text-white px-8 py-3 rounded-lg font-semibold hover:bg-gray-800 transition-colors">
                    Contact Us Now
                </NuxtLink>
            </section>
        </div>
    </div>
</template>

<script setup>
const books = [
    {
        title: "What To Do When Everything Goes Bad",
        image: "~/assets/img/what-to-do-when-everything-goes-bad-wilson-samson.jpg",
        link: "#" // Add actual purchase links
    },
    {
        title: "Engaged Employees, Thriving Business",
        image: "~/assets/img/engaged-employees-thriving-business-wilson-samson.jpg",
        link: "#"
    },
    {
        title: "Building a Thriving Organization",
        image: "~/assets/img/building-a-thriving-organization-wilson-samson.jpg",
        link: "#"
    },
    {
        title: "Only Quality People",
        image: "~/assets/img/only-quality-people-wilson-samson.jpg",
        link: "#"
    }
]
</script>

<style scoped>
.shadow-sm {
    box-shadow: 0 1px 3px 0 rgba(0, 0, 0, 0.1), 0 1px 2px 0 rgba(0, 0, 0, 0.06);
}
</style>