<template>
  <header class="header">
    <nav class="navbar is-fixed-bottom" role="navigation" aria-label="main navigation">
      <div class="navbar-menu">
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
      let nav = document.querySelector('#' + burger.dataset.target)

      burger.addEventListener('click', () => {
        burger.classList.toggle('is-active');
        nav.classList.toggle('is-active');
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
