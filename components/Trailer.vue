<template>
  <div class="trailer">
    <div class="iframe-container">
      <iframe
        width="560"
        height="315"
        src="https://www.youtube-nocookie.com/embed/_AuOkjvMNPE"
        frameborder="0"
        allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Trailer'
};
</script>

<style lang="scss">
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
</style>
