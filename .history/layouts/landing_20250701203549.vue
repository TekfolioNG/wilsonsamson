<template>
  <LandingNavbar></LandingNavbar>
  <slot></slot>
  <LandingFooter v-if="$route.path !== '/'"></LandingFooter>
</template>