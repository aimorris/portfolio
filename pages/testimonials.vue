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
          <p>
            Adam is an active maintainer on Exercism, working across a variety of tracks and leading development on PureScript. He has an keen attention to detail and a desire to see things done properly.
          </p>
          <br>
          <p class="author">Jeremy Walker, co-founder at <a target="_blank" rel="noopener noreferrer" href="https://exercism.io">Exercism</a></p>
        </div>
      </slide>
      <slide>
        <img src="~/assets/lichess.svg" alt="Exercism logo">
        <div class="text">
          <p>
            Providing front-end bug fixes as well as new UI/UX feature implementations, Adam has been a valuable contributor for the Lichess website.
          </p>
          <br>
          <p class="author">Thibault Duplessis, founder at <a target="_blank" rel="noopener noreferrer" href="https://lichess.org">Lichess</a></p>
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

      a {
        color: #191D32;
        text-decoration: underline;
      }

      p {
        font-size: 1em;
      }
    }
  }

  .author {
    font-weight: bold;
  }
</style>
