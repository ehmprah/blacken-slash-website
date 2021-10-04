<template>
  <div class="container">
    <div>
      <img class="logo" src="/logo.png" alt="Blacken Slash Logo" />

      <div class="about">
        <div class="about__description">
          The minimalist love child of turn based tactical and hack, slash and
          loot games. Fight, loot, repeat until you die. Perfect your gear
          across dozens of runs or compete in an online leaderboard where you
          start from scratch each week. A simple but deep, difficult and highly
          replayable game.
        </div>
      </div>

      <Buy />

      <div class="trailer">
        <div class="iframe-container">
          <iframe
            width="560"
            height="315"
            src="https://www.youtube-nocookie.com/embed/47SFM1lvpq4"
            frameborder="0"
            allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
      </div>

      <div class="screenshots">
        <h2>Screenshots</h2>
        <div class="screenshots__container">
          <Screenshot url="/img/01.png" />
          <Screenshot url="/img/02.png" />
          <Screenshot url="/img/03.png" />
          <Screenshot url="/img/04.png" />
          <Screenshot url="/img/05.png" />
          <Screenshot url="/img/06.png" />
          <Screenshot url="/img/07.png" />
          <Screenshot url="/img/08.png" />
        </div>
      </div>

      <div class="section">
        <h2>Follow</h2>
        <Follow />
      </div>

      <div class="section">
        <h2>Quick Facts</h2>
        <QuickFacts />
      </div>

      <div class="footer">
        <Navigation />
      </div>
    </div>
  </div>
</template>

<script>
import Buy from '~/components/Buy.vue';
import Follow from '~/components/Follow.vue';
import Navigation from '~/components/Navigation.vue';
import QuickFacts from '~/components/QuickFacts.vue';
import Screenshot from '~/components/Screenshot.vue';

export default {
  components: {
    Buy,
    Follow,
    Navigation,
    QuickFacts,
    Screenshot
  },
  head() {
    return {
      title: 'Core Defense'
    };
  }
};
</script>

<style lang="scss">
.logo {
  max-width: 512px;
  margin-top: 40px;
}

.about {
  width: 80vw;
  max-width: 520px;
  margin: 0 auto 40px auto;

  &__short {
    font-size: 1.25em;
  }

  &__description {
    text-align: justify;
    margin: 1em 0;
  }
}

.trailer {
  max-width: 720px;
  margin: 0 auto;
}

.iframe-container {
  position: relative;
  overflow: hidden;
  width: 100%;
  padding-top: 56.25%;

  iframe {
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    width: 100%;
    height: 100%;
  }
}

.screenshots {
  max-width: 960px;
  margin: 80px auto;
  &__container {
    display: flex;
    flex-wrap: wrap;
    .screenshot {
      flex: 1 0 200px;
    }
  }
}

.section {
  max-width: 640px;
  margin: 80px auto;
}

.newsletter {
  margin: 80px auto;
  &__info {
    font-size: 0.8em;
    color: #aaa;
  }
}

.footer {
  margin: 4em 0 2em 0;
}
</style>
