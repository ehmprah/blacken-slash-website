<template>
  <div>
    <div class="about">
      A nostalgic blast of tactical hack & slash action.<br />
      Fight, loot, upgrade, die ... repeat!
    </div>
    <Buy />
    <Trailer />

    <div class="section">
      <h2>Facts</h2>
      <QuickFacts />
    </div>

    <div class="section">
      <h2>Follow</h2>
      <Follow />
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
  </div>
</template>

<script>
import Buy from '~/components/Buy.vue';
import Follow from '~/components/Follow.vue';
import QuickFacts from '~/components/QuickFacts.vue';
import Screenshot from '~/components/Screenshot.vue';
import Trailer from '~/components/Trailer.vue';

export default {
  components: {
    Buy,
    Follow,
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
.about {
  width: 80vw;
  max-width: 520px;
  margin: 0 auto 50px auto;
  color: #f3c05e;
  text-shadow: 2px 2px 0 black;
  font-size: 20px;
  line-height: 1.5em;
}

ul.buy {
  margin: 0 auto 50px auto;
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
