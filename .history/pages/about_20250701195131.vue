<template>
    <div class="about-page">
        <!-- Social Media Icons (Sticky Right Side) -->
        <div class="social-media-sticky">
            <a href="#" class="social-icon" v-for="icon in socialIcons" :key="icon.name"
                :style="{ backgroundColor: icon.color }">
                <i :class="icon.iconClass"></i>
            </a>
        </div>

        <!-- Main Content -->
        <div class="container mx-auto px-4 py-12 md:py-20">
            <!-- Section 1 -->
            <div class="flex flex-col md:flex-row items-center gap-12 mb-24">
                <div class="md:w-1/2">
                    <img src="~/assets/img/wilsonsamson-hero-image4.png" alt="Wilson Samson professional portrait"
                        class="rounded-lg shadow-xl w-full h-auto object-cover" />
                </div>
                <div class="md:w-1/2">
                    <h1 class="text-4xl md:text-5xl font-bold mb-6 text-gray-800">About <span
                            class="text-primary">Wilson</span></h1>
                    <p class="text-lg text-gray-600 mb-4">
                        Wilson Samson is a visionary creative professional with over a decade of experience at the
                        intersection of design, technology, and storytelling. His unique approach blends technical
                        precision with artistic intuition to deliver exceptional results.
                    </p>
                    <p class="text-lg text-gray-600 mb-4">
                        Beginning his career in graphic design, Wilson quickly expanded his expertise into web
                        development, user experience, and digital strategy. This multidisciplinary background allows him
                        to bridge the gap between form and function.
                    </p>
                    <p class="text-lg text-gray-600">
                        When not pushing pixels or writing code, Wilson can be found mentoring young designers,
                        exploring new technologies, or searching for the perfect cup of coffee.
                    </p>
                </div>
            </div>

            <!-- Section 2 (Reversed) -->
            <div class="flex flex-col md:flex-row-reverse items-center gap-12 mb-24">
                <div class="md:w-1/2">
                    <img src="~/assets/img/wilsonsamson-about.jpg" alt="Wilson Samson at work"
                        class="rounded-lg shadow-xl w-full h-auto object-cover grayscale hover:grayscale-0 transition-all duration-500" />
                </div>
                <div class="md:w-1/2">
                    <h2 class="text-3xl md:text-4xl font-bold mb-6 text-gray-800">Philosophy & <span
                            class="text-primary">Approach</span></h2>
                    <p class="text-lg text-gray-600 mb-4">
                        Wilson believes that great design solves problems before users know they exist. His work is
                        guided by three core principles: clarity, purpose, and emotional resonance. Every project begins
                        with deep listening and ends with measurable impact.
                    </p>
                    <p class="text-lg text-gray-600 mb-4">
                        In an industry that often prioritizes trends over substance, Wilson champions timeless solutions
                        that grow with businesses. His collaborative process ensures clients become active partners in
                        creation, not just spectators.
                    </p>
                    <p class="text-lg text-gray-600">
                        The proof is in the portfolio - from Fortune 500 companies to passionate startups, Wilson's work
                        consistently delivers both aesthetic excellence and business results.
                    </p>
                </div>
            </div>

            <!-- Final Line -->
            <div class="text-center border-t border-gray-200 pt-8">
                <p class="text-gray-500 italic">
                    "Creating isn't just what I do - it's how I understand the world."
                </p>
            </div>
        </div>
    </div>
</template>

<script setup>
// Social media icons data
const socialIcons = [
    { name: 'twitter', iconClass: 'fab fa-twitter', color: '#1DA1F2' },
    { name: 'linkedin', iconClass: 'fab fa-linkedin-in', color: '#0077B5' },
    { name: 'dribbble', iconClass: 'fab fa-dribbble', color: '#EA4C89' },
    { name: 'github', iconClass: 'fab fa-github', color: '#333' },
    { name: 'behance', iconClass: 'fab fa-behance', color: '#1769FF' },
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

.text-primary {
    color: #4F46E5;
    /* Adjust to match your brand color */
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

/* Add this if you want scroll-triggered animations */
/* You'll need to implement the scroll detection logic */
.social-icon.animate {
    animation: pop 0.5s ease;
}
</style>