<template>
  <div id="main" v-bind:style="divStyle">
    <table id="content-table">
      <div class="center">
      <td>
        <img
          v-bind:src="img"
          v-bind:style="imgStyle"
          id="main-img"
          alt="main project image"
        />
      </td>
      <td style="vertical-align: top">
        <div id="text-div">
          <slot />
        </div>
      </td>
      </div>
    </table>
    <div id="background-div">
      <img
        v-bind:src="backgroundImg"
        id="background-img"
        alt="project background image"
      />
    </div>
  </div>
</template>
<script>
export default {
  props: ["img", "background-img", "side"],
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
  filter: brightness(30%);
  object-fit: cover;
  height: min(80vh + 50px, 40vw + 50px);
}
#main-img {
  height: min(80vh, 40vw);
}

p {
  font-size: min(3vh, 2vw);
}
h1 {
  font-size: min(6vh, 4vw);
}
a {
  font-size: min(3vh, 2vw);
  color: grey
}
</style>