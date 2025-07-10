<template>
  <LandingNavbar :is-dark-mode="$route.path !== '/'"></LandingNavbar>
  <slot></slot>
  <LandingFooter v-if="$route.path !== '/'"></LandingFooter>
</template>