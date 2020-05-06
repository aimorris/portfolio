<template>
  <div class="container">
    <div>
      <logo />
      <h1 class="title">
        Adam Morris
      </h1>
      <h2 class="subtitle">
        <vue-typer text="Hello world!"></vue-typer>
      </h2>
      <div class="links">
        <a href="https://github.com/aimorris" target="_blank" class="button--github">GitHub</a>
        <a href="https://gitlab.com/aimorris" target="_blank" class="button--gitlab">GitLab</a>
        <a href="https://bitbucket.com/aimorris" target="_blank" class="button--bitbucket">BitBucket</a>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
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
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
