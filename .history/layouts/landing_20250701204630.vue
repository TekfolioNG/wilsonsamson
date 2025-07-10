<template>
  <!-- Use LandingNavbar only for homepage, InvertedNavbar for other pages -->
  <LandingNavbar v-if="$route.path === '/'"></LandingNavbar>
  <InvertedNavbar v-else></InvertedNavbar>

  <slot></slot>

  <LandingFooter v-if="$route.path !== '/'"></LandingFooter>
</template>
