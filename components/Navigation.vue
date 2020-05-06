<template>
  <header class="header">
    <nav class="navbar is-fixed-top" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <a class="navbar-item" href="https://bulma.io">
          <img src="https://bulma.io/images/bulma-logo.png" width="112" height="28">
        </a>
        <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navigation-bar">
          <span aria-hidden="true" />
          <span aria-hidden="true" />
          <span aria-hidden="true" />
        </a>
      </div>
      <div id="navigation-bar" class="navbar-menu">
        <div class="navbar-start">
          <a href="/" class="navbar-item">Home</a>
          <a href="/projects" class="navbar-item">Projects</a>
          <a href="/about" class="navbar-item">About</a>
          <a href="/contact" class="navbar-item">Contact</a>
        </div>
      </div>
    </nav>
    <script>
      let burger = document.querySelector('.burger')
      let nav = document.querySelector('#' + burger.dataset.target)

      burger.addEventListener('click', function() {
        burger.classList.toggle('is-active');
        nav.classList.toggle('is-active');
      })
    </script>
  </header>
</template>
