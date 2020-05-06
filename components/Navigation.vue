<template>
  <header class="header">
    <nav class="navbar is-fixed-top" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target=".navbar-menu">
          <span aria-hidden="true" />
          <span aria-hidden="true" />
          <span aria-hidden="true" />
        </a>
      </div>
      <div class="navbar-menu">
        <div class="navbar-brand">
          <a href="https://github.com/aimorris" class="navbar-item navbar-github-icon"><font-awesome-icon :icon="['fab', 'github']" /></a>
          <a href="https://gitlab.com/aimorris" class="navbar-item"><font-awesome-icon :icon="['fab', 'gitlab']" /></a>
          <a href="https://bitbucket.com/aimorris" class="navbar-item"><font-awesome-icon :icon="['fab', 'bitbucket']" /></a>
        </div>
        <div class="navbar-end">
          <a href="/" class="navbar-item">Home</a>
          <a href="/projects" class="navbar-item">Projects</a>
          <a href="/about" class="navbar-item">About</a>
          <a href="/about" class="navbar-item">Testimonials</a>
          <a href="/contact" class="navbar-item">Contact</a>
        </div>
      </div>
    </nav>
    <script>
      let burger = document.querySelector('.burger')

      burger.addEventListener('click', function () {
        burger.classList.toggle('is-active')
        document.querySelector(burger.dataset.target).classList.toggle('is-active')
      })
    </script>
  </header>
</template>

<style lang="scss">
  .navbar-item {
    transition: color 0.3s;
    &:hover {
      color: #5D5D81;
    }
  }
</style>
