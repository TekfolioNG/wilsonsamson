<script setup lang="ts">
definePageMeta({
  layout: "landing"
});

useHead({
  title: 'Wilson Samson | Engineering, Real Estate & Procurement Services in Nigeria',
  meta: [
    {
      name: 'description',
      content:
        'Wilson Samson provides engineering, real estate, procurement, and project management services across Nigeria. Delivering innovative, reliable, and sustainable solutions for individuals and businesses.'
    },
    { property: 'og:title', content: 'Wilson Samson | Engineering, Real Estate & Procurement Services in Nigeria' },
    {
      property: 'og:description',
      content:
        'Engineering, construction, real estate, and procurement services across Nigeria. Wilson Samson delivers reliable and innovative solutions tailored to client needs.'
    },
    { property: 'og:image', content: 'https://wilsonsamson.com/og-image.jpg' },
    { property: 'og:image:width', content: '1200' },
    { property: 'og:image:height', content: '630' },
    { property: 'og:image:alt', content: 'Wilson Samson - Engineering, Real Estate & Procurement Solutions' },
    { name: 'twitter:card', content: 'summary_large_image' },
    { name: 'twitter:title', content: 'Wilson Samson | Engineering, Real Estate & Procurement Services' },
    {
      name: 'twitter:description',
      content:
        'Delivering trusted engineering, construction, real estate, and procurement services in Nigeria.'
    },
    { name: 'twitter:image', content: 'https://wilsonsamson.com/og-image.jpg' }
  ]
});

</script>

<template>
  <LandingContainer>
    <LandingHero></LandingHero>
  </LandingContainer>
</template>
