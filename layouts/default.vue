<template>
  <div>
    <Navigation />
    <client-only>
      <Particles />
    </client-only>
    <nuxt />
  </div>
</template>

<script>
import Navigation from '~/components/Navigation.vue'
import Particles from '~/components/Particles.vue'

export default {
  components: {
    Navigation,
    Particles
  }
}
</script>

<style>
html {
  /* font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif; */
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
  font-family: 'Raleway', sans-serif;
}

#particles-js {
  height: 100vh !important;
  width: 100vw !important;
  position: fixed !important;
  top: 0 !important;
  margin: 0 !important;
  padding: 0 !important;
  overflow: hidden !important;
  z-index: -1 !important;
}

.page-enter-active, .page-leave-active {
  transition: all 0.3s ease-in;
}

.page-enter, .page-leave-active {
  opacity: 0;
}
</style>
