<script setup lang="ts">
definePageMeta({
  layout: "landing"
});

useHead({
  title: 'Wilson Samson | Business Connector for Entrepreneurs & Professionals',
  meta: [
    {
      name: 'description',
      content:
        'Wilson Samson helps entrepreneurs and professionals unlock their strengths, bridge gaps between strategy and systems, and grow their impact through coaching, workshops, and business writing services.'
    },
    { property: 'og:title', content: 'Wilson Samson — Coaching · Strategy · Publishing Services' },
    {
      property: 'og:description',
      content:
        'Engineering, construction, real estate, and procurement services across Nigeria. Wilson Samson delivers reliable and innovative solutions tailored to client needs.'
    },
    { property: 'og:image', content: 'https://wilsonsamson.com/og-image.png' },
    { property: 'og:image:width', content: '1200' },
    { property: 'og:image:height', content: '630' },
    { property: 'og:image:alt', content: 'Guiding business leaders to clarity, productivity, and influence through strength-based coaching, strategy sessions, and publishing support.' },
    { name: 'twitter:card', content: 'summary_large_image' },
    {
      name: 'twitter:title', content: 'Wilson Samson | Business Connector for Entrepreneurs & Professionals'
    },
    {
      name: 'twitter:description',
      content:
        'Wilson Samson — Coaching · Strategy · Publishing Services'
    },
    { name: 'twitter:image', content: 'https://wilsonsamson.com/og-image.png' }
  ]
});

</script>

<template>
  <LandingContainer>
    <LandingHero></LandingHero>
  </LandingContainer>
</template>
