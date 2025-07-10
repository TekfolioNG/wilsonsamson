<template>
    <div class="about-page bg-white">
        <!-- Social Media Icons (Sticky Right Side) -->
        <div class="social-media-sticky">
            <a href="#" class="social-icon" v-for="icon in socialIcons" :key="icon.name"
                :style="{ backgroundColor: icon.color }">
                <i :class="icon.iconClass"></i>
            </a>
        </div>

        <!-- Main Content -->
        <div class="container mx-auto px-4 py-12 md:py-20">
            <!-- Hero Section -->
            <div class="flex flex-col md:flex-row items-center gap-12 mb-24">
                <div class="md:w-1/2">
                    <img src="~/assets/img/wilsonsamson-hero-image4.png" alt="Wilson Samson professional portrait"
                        class="rounded-lg shadow-xl w-full h-auto object-cover" />
                </div>
                <div class="md:w-1/2">
                    <h1 class="text-4xl md:text-5xl font-bold mb-6 text-gray-900">About <span
                            class="text-brand-blue">Wilson Samson</span></h1>
                    <p class="text-lg text-gray-700 mb-6">
                        Wilson Samson helps business owners reclaim their time, gain clarity, and lead with purpose. For
                        nearly two decades, he has worked with entrepreneurs and teams to build businesses that don't
                        depend on constant oversight, freeing leaders to focus on what truly matters.
                    </p>

                    <div class="bg-brand-blue/10 p-6 rounded-lg border-l-4 border-brand-blue mb-6">
                        <h3 class="font-semibold text-lg mb-2 text-gray-900">Credentials & Education</h3>
                        <ul class="space-y-2 text-gray-700">
                            <li class="flex items-start">
                                <span class="mr-2 text-brand-blue">•</span>
                                <span>Certified Professional in Enterprise Management (CPEM)</span>
                            </li>
                            <li class="flex items-start">
                                <span class="mr-2 text-brand-blue">•</span>
                                <span>Recipient of the UK's International Award in Delivering Training (IADT)</span>
                            </li>
                            <li class="flex items-start">
                                <span class="mr-2 text-brand-blue">•</span>
                                <span>B.Sc. in Psychology from Nnamdi Azikiwe University</span>
                            </li>
                            <li class="flex items-start">
                                <span class="mr-2 text-brand-blue">•</span>
                                <span>Alumnus of SKYE program (GIZ Germany) and Daystar Leadership Academy</span>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>

            <!-- Expertise Section -->
            <div class="flex flex-col md:flex-row-reverse items-center gap-12 mb-24">
                <div class="md:w-1/2">
                    <img src="~/assets/img/wilsonsamson-about.jpg" alt="Wilson Samson at work"
                        class="rounded-lg shadow-xl w-full h-auto object-cover grayscale hover:grayscale-0 transition-all duration-500" />
                </div>
                <div class="md:w-1/2">
                    <h2 class="text-3xl md:text-4xl font-bold mb-6 text-gray-900">Global <span
                            class="text-brand-blue">Impact</span></h2>
                    <p class="text-lg text-gray-700 mb-4">
                        Wilson offers a unique mix of clarity coaching, employee training, and strategic publishing —
                        helping business owners simplify operations, boost team performance, and grow their authority
                        without burning out.
                    </p>
                    <p class="text-lg text-gray-700 mb-6">
                        Over the past two decades, he has trained and empowered more than 10,000 professionals across
                        Nigeria, Ghana, Cameroon, Kenya, Zambia, South Africa, Liberia, the United States, and the
                        United Kingdom. His work cuts across multiple sectors, including oil and gas, tech, logistics,
                        real estate, construction, healthcare, education, and non-profits.
                    </p>

                    <div class="bg-gray-100 p-6 rounded-lg mb-6 border border-gray-200">
                        <h3 class="font-semibold text-lg mb-3 text-gray-900">Current Role</h3>
                        <p class="text-gray-700">
                            Chief Growth Officer and co-founder of Litera-Forge Ltd, a company he runs alongside his
                            wife, Abimbola.
                        </p>
                    </div>
                </div>
            </div>

            <!-- Core Values Section -->
            <div class="max-w-4xl mx-auto mb-24">
                <h2 class="text-3xl md:text-4xl font-bold mb-12 text-center text-gray-900">Core <span
                        class="text-brand-blue">Values</span></h2>

                <div class="grid md:grid-cols-2 gap-8">
                    <div v-for="value in coreValues" :key="value.title"
                        class="bg-white p-6 rounded-lg shadow-sm border-t-4 border-brand-blue hover:shadow-md transition-all">
                        <h3 class="text-xl font-bold mb-3 text-gray-900">{{ value.title }}</h3>
                        <p class="text-gray-700">{{ value.description }}</p>
                    </div>
                </div>
            </div>

            <!-- Volunteer Experience -->
            <div class="bg-gray-50 p-8 rounded-xl mb-12 border border-gray-200">
                <h3 class="text-2xl font-bold mb-6 text-center text-gray-900">Volunteer <span
                        class="text-brand-blue">Leadership</span></h3>
                <div class="flex flex-wrap justify-center gap-4">
                    <span v-for="org in volunteerOrgs" :key="org"
                        class="bg-white px-4 py-2 rounded-full text-sm font-medium shadow-sm border border-gray-200 hover:bg-brand-blue/10 transition-colors">
                        {{ org }}
                    </span>
                </div>
            </div>

            <!-- Final Line -->
            <div class="text-center border-t border-gray-200 pt-12">
                <p class="text-gray-600 italic text-lg">
                    "Creating systems that empower people to lead with clarity and purpose."
                </p>
            </div>
        </div>
    </div>
</template>

<script setup>
definePageMeta({
    layout: "landing"
})

// Brand color
const brandBlue = '#3b82f6'

// Social media icons data
const socialIcons = [
    { name: 'twitter', iconClass: 'fab fa-twitter', color: '#1DA1F2' },
    { name: 'linkedin', iconClass: 'fab fa-linkedin-in', color: '#0077B5' },
    { name: 'instagram', iconClass: 'fab fa-instagram', color: '#E1306C' },
    { name: 'youtube', iconClass: 'fab fa-youtube', color: '#FF0000' },
    { name: 'facebook', iconClass: 'fab fa-facebook-f', color: '#4267B2' },
]

// Core values data
const coreValues = [
    {
        title: 'Clarity',
        description: 'Every decision starts with a clear vision, not just busy work. Without clarity, action is just motion.'
    },
    {
        title: 'Ownership',
        description: 'Systems aren\'t just about control. They\'re what give you room to grow and breathe. You don\'t need to do everything, but you must lead with intent.'
    },
    {
        title: 'Simplicity',
        description: 'Build a business that reflects your values, not just your goals. Business growth doesn\'t need to be complex.'
    },
    {
        title: 'Empowerment',
        description: 'Teams thrive when they\'re trusted, trained, and allowed to lead. Real impact comes from helping others stand on their own.'
    },
    {
        title: 'Impact',
        description: 'Every strategy should serve people and move results. Your story and expertise can shift industries — if it\'s shared the right way.'
    }
]

// Volunteer organizations
const volunteerOrgs = [
    'Tony Elumelu Foundation',
    'Jobs Initiative Lagos (JIL)',
    'Youth Employment Agency (YEA) Ghana',
    'Ready-Set-Work',
    'LSETF',
    'BEDS',
    'GIZ Germany'
]
</script>

<style scoped>
.about-page {
    position: relative;
}

.social-media-sticky {
    position: fixed;
    right: 20px;
    top: 50%;
    transform: translateY(-50%);
    display: flex;
    flex-direction: column;
    gap: 15px;
    z-index: 50;
}

.social-icon {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    font-size: 18px;
    transition: all 0.3s ease;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.social-icon:hover {
    transform: scale(1.15) translateX(-5px);
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
}

.text-brand-blue {
    color: #3b82f6;
}

.bg-brand-blue {
    background-color: #3b82f6;
}

/* Animation for social icons on page scroll */
@keyframes pop {
    0% {
        transform: scale(1);
    }

    50% {
        transform: scale(1.2);
    }

    100% {
        transform: scale(1);
    }
}

/* Volunteer badges hover effect */
.bg-white:hover {
    border-color: #3b82f6;
}
</style>