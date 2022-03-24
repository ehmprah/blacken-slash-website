<template>
  <div class="container">
    <div>
      <a href="/" class="logo">
        <img src="/logo/steam_library_logo.png" alt="Blacken Slash Logo" />
      </a>

      <Nuxt />

      <div class="footer">
        <Navigation />
      </div>
    </div>
  </div>
</template>

<script>
import Navigation from '~/components/Navigation.vue';

export default {
  components: {
    Navigation
  }
};
</script>

<style lang="scss">
html,
body,
p,
ol,
ul,
li,
dl,
dt,
dd,
blockquote,
figure,
fieldset,
legend,
textarea,
pre,
iframe,
hr,
h1,
h2,
h3,
h4,
h5,
h6 {
  margin: 0;
  padding: 0;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-size: 100%;
  font-weight: normal;
}

ul {
  list-style: none;
}

button,
input,
select,
textarea {
  margin: 0;
}

html {
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: inherit;
}

img,
svg,
embed,
object,
audio,
video {
  height: auto;
  max-width: 100%;
}

iframe {
  border: 0;
}

table {
  border-collapse: collapse;
  border-spacing: 0;
}

td,
th {
  padding: 0;
  text-align: left;
}

html {
  font-family: 'Rubik', sans-serif;
  font-size: 16px;
  line-height: 1.5em;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background: linear-gradient(45deg, #070b11, #0f1a27);
  color: #aaa;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

a,
a:hover {
  text-decoration: none;
  transition: all 0.2s;
  border-bottom: 1px solid;
  color: #ff1690;
}

a:hover {
  border-color: transparent;
}

p {
  margin-bottom: 1em;
}

h1,
h2 {
  // font-family: 'Wendy One', sans-serif;
  font-size: 2em;
  text-transform: uppercase;
  margin-bottom: 1em;
  color: #f3c05e;
  text-shadow: 4px 4px 0 #000;
}

ul.list {
  padding-left: 1.5em;
  list-style-type: circle;
  text-align: left;
}

ul.list-inline {
  li {
    display: inline;
    margin: 0.5em;
  }
}

ul.list-flex {
  list-style-type: circle;
  display: flex;
  flex-wrap: wrap;
  li {
    flex: 1 0 100%;
    width: 100%;
    max-width: 240px;
    text-align: left;
  }
}

.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.logo {
  display: block;
  width: 100%;
  max-width: 360px;
  margin: 0 auto;
  border: none !important;
}
</style>
