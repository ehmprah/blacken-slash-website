<template>
  <nav>
    <ul class="navigation">
      <li><a href="/">Home</a></li>
      <li><a href="/presskit">Presskit</a></li>
      <li><a href="/privacy-policy">Privacy Policy</a></li>
      <li><a href="/imprint">Imprint</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Navigation'
};
</script>

<style lang="scss">
ul.navigation {
  padding: 0;
  list-style-type: none;
  text-align: center;
  li {
    margin: 0.5em;
  }
}

@media only screen and (min-width: 600px) {
  ul.navigation {
    li {
      display: inline;
    }
  }
}
</style>
