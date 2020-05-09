<template>
  <div class="container">
    <carousel
      :perPage="1"
      :paginationEnabled="false"
      :navigationEnabled="true"
      :navigationNextLabel="'>'"
      :navigationPrevLabel="'<'"
    >
      <slide>
        <img src="~/assets/exercism.svg" alt="Exercism logo">
        <div class="text">
          <h1>Exercism V3</h1>
          <br>
          <p>
            I currently maintain the PureScript, CoffeeScript, JavaScript, and Haskell V3 tracks. I am leading the development of the PureScript track.
          </p>
          <br>
          <a target="_blank" rel="noopener noreferrer" href="https://github.com/exercism/v3" class="button--custom">GitHub</a>
        </div>
      </slide>

      <slide>
        <img src="~/assets/exercism.svg" alt="Exercism logo">
        <div class="text">
          <h1>Exercism V2 Solutions</h1>
          <br>
          <p>
            My solutions to Exercism V2 problems in various programming languages.
          </p>
          <br>
          <a target="_blank" rel="noopener noreferrer" href="https://github.com/aimorris/exercism-v2-solutions" class="button--custom">GitHub</a>
          <a target="_blank" rel="noopener noreferrer" href="https://exercism.io" class="button--custom">Site</a>
        </div>
      </slide>

      <slide>
        <img src="~/assets/flightscope.png" alt="Flightscope Aviation logo" style="width: 100%">
        <div class="text">
          <h1>Flightscope Aviation Website</h1>
          <br>
          <p>
            I developed the Flightscope Aviation website from scratch using HTML, CSS, JavaScript, and some minimal JQuery.
          </p>
          <br>
          <a target="_blank" rel="noopener noreferrer" href="https://gitlab.com/flightscope/flightscopeaviation.com.au" class="button--custom">GitLab</a>
          <a target="_blank" rel="noopener noreferrer" href="https://flightscope.gitlab.io/flightscopeaviation.com.au" class="button--custom">Site</a>
        </div>
      </slide>

      <slide>
        <img src="~/assets/lichess.svg" alt="Lichess logo">
        <div class="text">
          <h1>Lichess</h1>
          <br>
          <p>
            I have contributed to the Lichess website by providing new user interface features including bug fixes.
          </p>
          <br>
          <a target="_blank" rel="noopener noreferrer" href="https://github.com/ornicar/lila" class="button--custom">GitHub</a>
          <a target="_blank" rel="noopener noreferrer" href="https://lichess.org" class="button--custom">Site</a>
        </div>
      </slide>

      <slide>
        <img src="~/assets/upenn.png" alt="University of Pennsylvania logo">
        <div class="text">
          <h1>CIS194 Solutions</h1>
          <br>
          <p>
            My solutions to the University of Pennsylvania's CIS194 Spring 2013 course.
          </p>
          <br>
          <a target="_blank" rel="noopener noreferrer" href="https://github.com/aimorris/cis194" class="button--custom">GitHub</a>
          <a target="_blank" rel="noopener noreferrer" href="https://www.cis.upenn.edu/~cis194/spring13" class="button--custom">Site</a>
        </div>
      </slide>

      <slide>
        <img src="~/assets/game-of-life.gif" alt="Game of Life logo">
        <div class="text">
          <h1>TroTae's implementation of Conway's Game of Life</h1>
          <br>
          <p>
            I have implemented new patterns for TroyTae's implementation of Conway's Game of Life for the web, written in TypeScript.
          </p>
          <br>
          <a target="_blank" rel="noopener noreferrer" href="https://github.com/troytae/game-of-life" class="button--custom">GitHub</a>
          <a target="_blank" rel="noopener noreferrer" href="https://troytae.github.io/game-of-life" class="button--custom">Site</a>
        </div>
      </slide>

      <slide>
        <img src="~/assets/minecraft.png" alt="Minecraft logo">
        <div class="text">
          <h1>Virtual Enchant</h1>
          <br>
          <p>
            A Minecraft plugin that provides a virtual enchanting table via a command.
          </p>
          <br>
          <a target="_blank" rel="noopener noreferrer" href="https://github.com/aimorris/virtual-enchant" class="button--custom">GitHub</a>
          <a target="_blank" rel="noopener noreferrer" href="https://www.spigotmc.org/resources/virtual-enchant.78560/" class="button--custom">Spigot</a>
        </div>
      </slide>

      <slide>
        <img src="~/assets/minecraft.png" alt="Minecraft logo">
        <div class="text">
          <h1>Time Changer</h1>
          <br>
          <p>
            A Minecraft plugin that provides a GUI to change the world time.
          </p>
          <br>
          <a target="_blank" rel="noopener noreferrer" href="https://github.com/aimorris/time-changer" class="button--custom">GitHub</a>
          <a target="_blank" rel="noopener noreferrer" href="https://www.spigotmc.org/resources/timechanger.77522/" class="button--custom">Spigot</a>
        </div>
      </slide>

      <slide>
        <img src="~/assets/minecraft.png" alt="Minecraft logo">
        <div class="text">
          <h1>Flaming Head</h1>
          <br>
          <p>
            A Minecraft plugin that provides a flaming head particle effect.
          </p>
          <br>
          <a target="_blank" rel="noopener noreferrer" href="https://github.com/aimorris/flaming-head" class="button--custom">GitHub</a>
          <a target="_blank" rel="noopener noreferrer" href="https://www.spigotmc.org/resources/flaming-head.77690/" class="button--custom">Spigot</a>
        </div>
      </slide>

    </carousel>
  </div>
</template>

<style lang="scss">
  .VueCarousel {
    width: 100vw;
    .VueCarousel-navigation-button {
      font-size: 3vw;
      color: #191D32;
      transition: color 0.3s;
      outline: none;
    }

    .VueCarousel-slide {
      display: grid;
      grid-template-columns: 1fr 6fr;
      width: 10vw;
      padding: 0 5vw;
      align-items: center;
      text-align: center;

      img {
        height: auto;
        width: 80%;
      }

      p {
        font-size: 1em;
      }

      h1 {
        font-weight: bold;
      }

      .button--custom {
        text-decoration: none;
        padding: 1vw 3vw;
        margin: 0 1.5vw;
        display: inline-block;
        border-radius: 4px;
        border: 1px solid;
        border-color: #666;
        color: #666;

        transition: all 0.2s;
      }

      .button--custom:hover {
        color: #fff;
        background-color: #666;
      }
    }
  }

  .author {
    font-weight: bold;
  }
</style>
