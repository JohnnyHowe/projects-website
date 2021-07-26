<template>
  <div>
    <ProjectCard
      :img="require('@/assets/tower-dropper/screenshot.webp')"
      :video="require('@/assets/tower-dropper/gameplay.mp4')"
      ><h1>Tower Dropper</h1>
      <br />
      <p>
        Tower dropper is a mobile stacking game. The higher you build the tower,
        the more points you get.<br />
        Watch out though, some dumbass keeps loading up the crane with TNT. Who
        thought it would be a good idea to store TNT with the buildings?
      </p>
      <br />
      <a
        href="https://play.google.com/store/apps/details?id=com.DefaultCompany.TowerDropper&pcampaignid=pcampaignidMKT-Other-global-all-co-prtnr-py-PartBadge-Mar2515-1"
        target="_blank"
        ><img
          class="google-play"
          alt="Get it on Google Play"
          src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png"
      /></a>
    </ProjectCard>
    <ProjectCard
      :img="require('@/assets/jump/screenshot.png')"
      :video="require('@/assets/jump/gameplay.mp4')"
      ><h1>Jump</h1>
      <br />
      <p>
        Climb your way up higher and higher by launching yourself from wall to
        wall. <br />
        Don't take too long though, if you're too slow the acid will catch up
        and your game will be over.
      </p>
      <a
        href="https://play.google.com/store/apps/details?id=com.UnluckyDuck.Jump"
        target="_blank"
        ><img
          class="google-play"
          alt="Get it on Google Play"
          src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png"
      /></a>
    </ProjectCard>
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
<style scoped>
.google-play {
  height: min(10vh, 5vw);
}
</style>