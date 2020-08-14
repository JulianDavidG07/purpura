<template>
  <div class="container">
    <video class="container__video" autoplay muted loop>
      <source :src="require('../assets/video.mp4')" type="video/mp4" />
      Your browser does not support HTML5 video.
    </video>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container__video {
  position: absolute;
  top: 0;
  left: 0;
  display: block;
  width: 100vw;
  height: 100vh;
  object-fit: cover;
  z-index: 0;
}
</style>
