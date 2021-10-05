<template>
  <ul class="buy">
    <li>
      <a href="https://store.steampowered.com/app/1746560/Blacken_Slash/">
        <img src="/badges/steam.png" alt="Wishlist Blacken Slash on Steam" />
      </a>
    </li>
    <li>
      <a href="#" class="disabled">
        <img
          src="/badges/google-play.png"
          alt="Get Blacken Slash on Google Play"
        />
      </a>
      <div>soon&trade;</div>
    </li>
    <li>
      <a href="#" class="disabled">
        <img
          src="/badges/app-store.png"
          alt="Get Blacken Slash on the App Store"
        />
      </a>
      <div>soon&trade;</div>
    </li>
    <li>
      <a href="#" class="disabled">
        <img src="/badges/itchio.png" alt="Buy Blacken Slash on itch.io" />
      </a>
      <div>soon&trade;</div>
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
    a {
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
