<template>
  <div>
    <div v-for="i in 1" :key="i">
    <ProjectCard
      :img="require('@/assets/' + 'tower-dropper/' + 'screenshot.webp' + '')"
      :video="require('@/assets/' + 'tower-dropper/' + 'gameplay.mp4' + '')"
      :background-img="
        require('@/assets/' + 'tower-dropper/' + 'gameplay.gif' + '')
      "
      :backgroundVideo="require('@/assets/' + 'tower-dropper/' + 'gameplay.mp4' + '')"
      ><h1>Tower Dropper</h1>
      <br />
      <p>
        Tower dropper is a mobile stacking game. The higher you build the tower, the more points you get.<br/>
        Watch out though, some dumbass keeps loading up the crane with TNT. Who thought it would be a good idea to store TNT with the buildings?
      </p>
      <br />
      <a target="_blank" href="https://play.google.com/store/apps/details?id=com.DefaultCompany.TowerDropper">Tower Dropper on Google Play Store</a>
    </ProjectCard>
    <ProjectCard
      :img="require('@/assets/' + 'jump/' + 'screenshot.png' + '')"
      :background-img="require('@/assets/' + 'jump/' + 'background.png' + '')"
      ><h1>Jump</h1>
      <br />
      <p>
        I'll have two number 9s, a number 9 large, a number 6 with extra dip, a number 7, two number 45s, one with cheese, and a large soda
      </p>
    </ProjectCard>
  </div>
  </div>
</template>
<script>
import ProjectCard from "./ProjectCard.vue";

export default {
  components: {
    ProjectCard,
  },
};
</script>