<template>
  <div class="container">
    <client-only>
      <Particles />
    </client-only>
    <div>
      <h1 class="title">
        Adam Morris
      </h1>
      <h2 class="subtitle">
        I am a
        <vue-typer
          :text="['web developer', 'Minecraft plugin creator', 'contributor for open-source projects']"
          :shuffle="true"
          caret-animation="smooth"
          :erase-delay="100"
          erase-style="backspace"
        />
      </h2>
      <div class="links">
        <a href="https://github.com/aimorris" target="_blank" class="button--custom button--github">GitHub</a>
        <a href="https://gitlab.com/aimorris" target="_blank" class="button--custom button--gitlab">GitLab</a>
        <a href="https://bitbucket.com/aimorris" target="_blank" class="button--custom button--bitbucket">BitBucket</a>
      </div>
    </div>
  </div>
</template>

<script>
import Particles from '~/components/Particles.vue'

export default {
  components: {
    Particles
  }
}
</script>

<style lang="scss">

.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 5vw;
  color: #191D32;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 3vw;
  color: #38405F;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.vue-typer .custom.char.typed, .vue-typer .custom.caret {
  color: #38405F;
}

.links {
  padding-top: 15px;
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
</style>
