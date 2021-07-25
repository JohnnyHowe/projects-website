<template>
  <div id="app">
    <ProjectsPage />
  </div>
</template>

<script>
import ProjectsPage from "@/components/ProjectsPage.vue";

export default {
  name: "App",
  components: {
    ProjectsPage,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}
* {
  font-family: "Calibri";
  margin: 0px;
  padding: 0px;
}
</style>
