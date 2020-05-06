<template>
  <div>
    <Navigation />
    <nuxt />
  </div>
</template>

<script>
import Navigation from '~/components/Navigation.vue'
export default {
  components: {
    Navigation
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
  padding: 10px 30px;
  margin-left: 15px;
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
</style>
