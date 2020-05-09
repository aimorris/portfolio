<template>
  <transition appear>
    <div class="container">
      <div>
        <h1 class="title">
          Adam Morris
        </h1>
        <h2 class="subtitle">
          I am a
          <vue-typer
            :text="['web developer', 'contributor for open-source projects', 'front-end developer', 'freelancer']"
            caret-animation="smooth"
            :erase-delay="100"
            erase-style="backspace"
            initial-action='erasing'
          />
        </h2>
        <div class="links">
          <a target="_blank" rel="noopener noreferrer" href="https://github.com/aimorris" class="button--custom button--github">GitHub</a>
          <a target="_blank" rel="noopener noreferrer" href="https://gitlab.com/aimorris" class="button--custom button--gitlab">GitLab</a>
          <a target="_blank" rel="noopener noreferrer" href="https://bitbucket.com/aimorris" class="button--custom button--bitbucket">BitBucket</a>
        </div>
      </div>
    </div>
  </transition>
</template>

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
  display: block;
  font-weight: 500;
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

.vue-typer .custom.char.typed {
  color: #38405F;
}

.custom.caret {
  background-color: #38405F;
}

.links {
  padding-top: 15px;
}

.button--custom {
  text-decoration: none;
  padding: 1vw 3vw;
  margin: 0 1.5vw;
  display: inline-block;
  border-radius: 4px;
  border: 1px solid;

  transition: all 0.2s;
}

.button--github {
  border-color: #666;
  color: #666;
}

.button--github:hover {
  color: #fff;
  background-color: #666;
}

.button--gitlab {
  border-color: #FC6D27;
  color: #FC6D27;
}

.button--gitlab:hover {
  color: #fff;
  background-color: #FC6D27;
}

.button--bitbucket {
  border-color: #2684FF;
  color: #2684FF;
}

.button--bitbucket:hover {
  color: #fff;
  background-color: #2684FF;
}
</style>
