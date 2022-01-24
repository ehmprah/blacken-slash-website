<template>
  <div class="container">
    <div>
      <h1 class="title">Blacken Slash Privacy Policy</h1>

      <div class="text">
        <p>
          Blacken Slash does not collect any data on any platform.
        </p>
        <p>
          Competing in the online ladder mode only submits the nickname you have
          entered and a randomly generated user ID.
        </p>
        <h2>Contact Us</h2>
        <p>
          If you have any questions or suggestions about my Privacy Policy, do
          not hesitate to contact me at ehmprah@gmail.com.
        </p>
      </div>
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
  },
  head() {
    return {
      title: 'Blacken Slash Privacy Policy'
    };
  }
};
</script>

<style lang="scss">
.title {
  margin-top: 2em;
  line-height: 1.5em;
  font-size: 2em;
}

.text {
  width: 80vw;
  max-width: 640px;
  margin: 0 auto 80px auto;
  text-align: justify;
}

h2 {
  margin-top: 1em;
}

ul.list {
  margin-bottom: 1em;
}

.footer {
  margin: 4em 0 2em 0;
}
</style>
