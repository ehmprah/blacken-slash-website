<template>
  <ul class="buy">
    <li>
      <a
        class="badge"
        href="https://store.steampowered.com/app/1746560?utm_source=website"
      >
        <img src="/badges/steam.png" alt="Wishlist Blacken Slash on Steam" />
      </a>
    </li>
    <li>
      <a
        class="badge"
        href="https://apps.apple.com/app/blacken-slash-lite/id1605374559"
      >
        <img
          src="/badges/app-store.png"
          alt="Get Blacken Slash on the App Store"
        />
      </a>
    </li>
    <li>
      <a
        class="badge"
        href="https://play.google.com/store/apps/details?id=com.ehmprah.blackenslash.demo"
      >
        <img
          src="/badges/google-play.png"
          alt="Get Blacken Slash on Google Play"
        />
      </a>
    </li>
    <li>
      <a class="badge" href="https://ehmprah.itch.io/blacken-slash">
        <img src="/badges/itchio.png" alt="Buy Blacken Slash on itch.io" />
      </a>
    </li>
  </ul>
</template>

<script>
export default {
  name: 'Buy'
};
</script>

<style lang="scss">
ul.buy {
  margin: 60px auto;
  max-width: 700px;
  padding: 0;
  list-style-type: none;

  li {
    max-width: 200px;
    margin: 0 auto 20px auto;
    a.badge {
      display: block;
      border-bottom: none;
      transition: all 0.1s;
      &:hover {
        transform: scale(1.05);
      }
      &.disabled {
        pointer-events: none;
        cursor: default;
        opacity: 0.35;
      }
    }
    img {
      display: block;
    }
    .mt {
      margin-top: 5px;
    }
  }
}

@media only screen and (min-width: 600px) {
  ul.buy {
    display: flex;
    justify-content: center;
    li {
      margin: 0 0.5em;
    }
  }
}
</style>
