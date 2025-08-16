<script setup lang="ts">
definePageMeta({
  layout: "landing"
});

useHead({
  meta: [
    {
      property: 'og:title',
      content: 'Wilson Samson | Business Connector for Entrepreneurs & Professionals'
    },
    {
      property: 'og:description',
      content: 'Wilson Samson helps entrepreneurs and professionals unlock their strengths, bridge gaps between strategy and systems, and grow their impact through coaching, workshops, and business writing services.'
    },
    {
      property: 'og:image',
      content: 'https://wilsonsamson.com/og-image.png'
    },
    { property: 'og:image:width', content: '1200' },
    { property: 'og:image:height', content: '630' },
    {
      property: 'og:image:alt',
      content: 'Wilson Samson – Empowering Business Leaders'
    },
    { name: 'twitter:card', content: 'summary_large_image' },
    {
      name: 'twitter:title',
      content: 'Wilson Samson | Coach · Strategist · Author'
    },
    {
      name: 'twitter:description',
      content: 'Guiding business leaders to clarity, productivity, and influence through strength-based coaching, strategy sessions, and publishing support.'
    },
    { name: 'twitter:image', content: 'https://wilsonsamson.com/og-image.png' }
  ],
  title: 'Wilson Samson | Business Connector for Entrepreneurs & Professionals',
  metaTitle: 'Wilson Samson — Coaching · Strategy · Publishing Services',
  metaDescription: 'Wilson Samson helps professionals and entrepreneurs align their strengths, systems, and strategy with tailored discovery sessions, executive coaching, workshops, and ghostwriting services.',
});

</script>

<template>
  <LandingContainer>
    <LandingHero></LandingHero>
  </LandingContainer>
</template>
