<template>
  <header class="header">
    <nav class="navbar is-fixed-top" role="navigation" aria-label="main navigation">
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
