<template>
  <div id="main" v-bind:style="divStyle">
    <table id="content-table">
      <div class="center">
        <td>
          <Animated v-bind:video="video" v-bind:image="img" id="main-img" />
        </td>
        <td style="vertical-align: top">
          <div id="text-div">
            <slot />
          </div>
        </td>
      </div>
    </table>
    <div id="background-div">
      <Animated v-bind:video="video" v-bind:image="img" id="background-img" />
    </div>
  </div>
</template>
<script>
import Animated from "./Animated.vue";
export default {
  components: {
    Animated,
  },
  props: {
    img: { type: String },
    backgroundImg: { type: String },
    video: { type: String },
    backgroundVideo: { type: String },
  },
  computed: {
    imgStyle() {
      return `float: ${this.side}`;
    },
    divStyle() {
      return `text-align: ${this.side}`;
    },
  },
};
</script>
<style scoped>
.center {
  margin: auto;
  width: min(200vh, 80vw);
}
#main {
  position: relative;
  overflow: hidden;
}
#content-table {
  position: absolute;
  padding: 10px;
  width: 100%;
}
td {
  padding: 10px;
}
#background-div {
  position: relative;
  z-index: -1;
  top: 0px;
  left: 0px;
  height: min(80vh + 50px, 40vw + 50px);
}
#text-div {
  position: relative;
  text-align: left;
  color: white;
  vertical-align: top;
}
#background-img {
  left: 0px;
  top: 0px;
  width: 100%;
  filter: brightness(10%);
  object-fit: cover;
  height: min(80vh + 50px, 40vw + 50px);
}
#main-img {
  height: min(80vh, 40vw);
  width: min((9/16) * 80vh, (9/16) * 40vw);
}

p {
  font-size: min(3vh, 2vw);
}
h1 {
  font-size: min(6vh, 4vw);
}
a {
  font-size: min(3vh, 2vw);
  color: grey;
}
</style>