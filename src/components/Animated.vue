<template>
  <div>
    <video v-if="video" class="content" autoplay loop muted>
      <source :src="video" type="video/mp4" />
      <img class="content" v-bind:src="image" alt="main project image" />
    </video>
    <img v-else class="content" v-bind:src="image" alt="main project image" />
  </div>
</template>
<script>
/**
 * Component used for showing animated things.
 * If supplied with and client supports it, will prefer to show video, otherwise image.
 * Videos are shown with no controls, they autoplay and loop, so they appear like a gif.
 * Content will grow to take up max vertical space allowed
 */
export default {
  props: ["video", "image"],
};
</script>
<style scoped>
.content {
  width: 100%;
  height: 100%;
  object-fit: inherit;
}
</style>