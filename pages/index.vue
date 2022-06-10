<template>
  <div>
    <div class="about">
      A tactical roguelite RPG where the items you choose define your character.
      Create powerful builds from an abundance of loot as you try to save a
      corrupted retro computer system in bite-sized tactical puzzles.
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
  </div>
</template>

<script>
import Buy from '~/components/Buy.vue';
import Follow from '~/components/Follow.vue';
import Screenshot from '~/components/Screenshot.vue';
import Trailer from '~/components/Trailer.vue';

export default {
  components: {
    Buy,
    Follow,
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
  color: #ff1690;
  text-shadow: 2px 2px 0 black;
  font-size: 18px;
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
