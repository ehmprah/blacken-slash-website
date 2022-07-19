<template>
  <div class="container">
    <div>
      <h1 class="title">PRESSKIT</h1>

      <div class="text">
        <h2>History</h2>
        <div class="text__description">
          After creating "one of the best tower defense games"
          <sup
            >(<a
              href="https://apps.apple.com/us/app/core-defense/id1546364145#see-all/reviews"
              >1</a
            >,
            <a
              href="https://steamcommunity.com/profiles/76561198844316377/recommended/1203360/"
              >2</a
            >,
            <a href="https://steamcommunity.com/id/Crytch/recommended/1203360/"
              >3</a
            >,
            <a
              href="https://steamcommunity.com/profiles/76561198031887977/recommended/1203360/"
              >4</a
            >,
            <a
              href="https://steamcommunity.com/profiles/76561197992239750/recommended/1203360/"
              >5</a
            >,
            <a href="https://steamcommunity.com/id/j0maK/recommended/1203360/"
              >6</a
            >,
            <a
              href="https://steamcommunity.com/profiles/76561198437756055/recommended/1203360/"
              >7</a
            >)</sup
          >
          with <a href="https://coredefense.ehmprah.com/">Core Defense</a>, solo
          indie developer Mario "ehmprah" Kaiser is setting out to create yet
          another minimalist, unexpected fusion of game genres with Blacken
          Slash.
        </div>
      </div>

      <div class="text">
        <h2>Description</h2>
        <div class="text__description">
          A tactical RPG fusing the best of roguelikes, turn-based tactics and
          hack and slash games – made by a solo developer with a penchant for
          minimalist designs.
        </div>
        <ul class="list">
          <li>Fight through bite-sized tactical puzzles</li>
          <li>
            Create powerful builds from a plethora of items which grant you
            skills and can change gameplay mechanics
          </li>
          <li>Carry on your favorite items between runs in normal mode</li>
          <li>
            Start from scratch each week and compete with other players in the
            online ladder mode
          </li>
          <li>Try various playstyles and hunt for challenging achievements</li>
          <li>
            Enjoy a lovingly crafted story of ridiculous computer nostalgia and
            a blast of a retro soundtrack
          </li>
        </ul>
      </div>

      <Trailer />

      <div class="screenshots">
        <h2>Screenshots</h2>
        <p><a href="/img/blacken_slash_screenshots.zip">Download as .zip</a></p>
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

      <div class="logos">
        <h2>Logos & Key Art</h2>
        <p><a href="/logo/blacken_slash_logos.zip">Download as .zip</a></p>
        <div class="logos__container">
          <img class="logo" src="/logo/blacken_slash_1920x1080.png" />
          <img class="logo" src="/logo/blacken_slash_box_art.png" />
          <img class="logo" src="/logo/blacken_slash_key_art_a.png" />
          <img class="logo" src="/logo/blacken_slash_key_art_b.png" />
          <img class="logo" src="/logo/blacken_slash_logo_transparent.png" />
        </div>
      </div>

      <div class="section">
        <h2>Facts</h2>
        <QuickFacts />
      </div>

      <div class="section">
        <h2>Links</h2>
        <ul class="list links">
          <li>
            <a
              href="https://store.steampowered.com/app/1746560?utm_source=presskit"
              >Steam</a
            >
          </li>
          <li>
            <a
              href="https://play.google.com/store/apps/details?id=com.ehmprah.blackenslash"
              >Play Store</a
            >
          </li>
          <li>
            <a
              href="https://play.google.com/store/apps/details?id=com.ehmprah.blackenslash.demo"
              >Play Store (Demo)</a
            >
          </li>
          <li>
            <a href="https://apps.apple.com/app/blacken-slash/id1604646442"
              >App Store</a
            >
          </li>
          <li>
            <a href="https://apps.apple.com/app/blacken-slash-lite/id1605374559"
              >App Store (Demo)</a
            >
          </li>
          <li><a href="https://blackenslash.ehmprah.com/">Website</a></li>
          <li><a href="https://discord.gg/y9hjQndJS2">Discord</a></li>
          <li><a href="https://twitter.com/ehmprah">Twitter</a></li>
        </ul>
      </div>

      <div class="section">
        <h2>Mentions</h2>
        <p>
          "I really liked what ehmprah did with Core Defense, and I am a fan of
          distilling design down to its core and this looks really tight."<br />–
          <a
            href="https://twitter.com/TheStrategyInf1/status/1446270183350362119"
            >The Strategy Informer</a
          >
        </p>
        <p>
          "Honestly I think that there's a lot of promise here"<br />–
          <a href="https://www.youtube.com/watch?v=cNz7Mc1ekJc">Retromation</a>
        </p>
        <p>
          "It's so satisfying."<br />–
          <a href="https://youtu.be/h4lbmour2Lo?t=1651">Olexa</a>
        </p>
      </div>

      <div class="section">
        <h2>Contact</h2>
        Send a mail to <a href="mailto:ehmprah@gmail.com">ehmprah@gmail.com</a>
      </div>
    </div>
  </div>
</template>

<script>
import QuickFacts from '~/components/QuickFacts.vue';
import Screenshot from '~/components/Screenshot.vue';
import Trailer from '~/components/Trailer.vue';

export default {
  components: {
    QuickFacts,
    Screenshot,
    Trailer
  },
  head() {
    return {
      title: 'Presskit "Blacken Slash"'
    };
  }
};
</script>

<style lang="scss">
.title {
  margin: 0 0 1em;
  line-height: 1.5em;
  font-size: 3em;
}

.text {
  width: 80vw;
  max-width: 640px;
  margin: 0 auto 50px auto;
  &__description {
    text-align: left;
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
  &--gif {
    .screenshot {
      flex: 1 0 300px;
    }
  }
}

.logos {
  &__container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    .logo {
      display: block;
      margin: 1em auto;
      max-width: 180px;
      height: auto;
    }
  }
}

.links {
  max-width: 480px;
  margin: 0 auto;
}

.section {
  max-width: 600px;
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
