<template>
  <div class="container">
    <div>
      <img class="logo" src="/logo.svg" alt="Blacken Slash Logo" />

      <div class="about">
        <div class="about__description">
          Return the rogue colors to the prismatic fold! Fight, loot, improve
          your gear, repeat. Hack and slash meets turn based tactics, seasoned
          with roguelite elements and distilled until there's nothing but fun
          left. Difficult and highly replayable.
        </div>
      </div>

      <Buy />

      <Trailer />

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
import Trailer from '~/components/Trailer.vue';

export default {
  components: {
    Buy,
    Follow,
    Navigation,
    QuickFacts,
    Screenshot,
    Trailer
  },
  head() {
    return {
      title: 'Blacken Slash'
    };
  }
};
</script>

<style lang="scss">
.logo {
  width: 100%;
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
