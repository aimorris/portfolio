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
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
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
}

.button--custom {
  text-decoration: none;
  padding: 1vw 3vw;
  margin: 0 1.5vw;
  display: inline-block;
  border-radius: 4px;

  transition: all 0.2s;
}

.button--github {
  border: 1px solid #666;
  color: #666;
}

.button--github:hover {
  color: #fff;
  background-color: #666;
}

.button--gitlab {
  border: 1px solid #FC6D27;
  color: #FC6D27;

  transition:
}

.button--gitlab:hover {
  color: #fff;
  background-color: #FC6D27;
}

.button--bitbucket {
  border: 1px solid #2684FF;
  color: #2684FF;
}

.button--bitbucket:hover {
  color: #fff;
  background-color: #2684FF;
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
  transition: all .30s ease-out;
}

.page-enter, .page-leave-active {
  opacity: 0;
  transform-origin: 50% 50%;
}
</style>
