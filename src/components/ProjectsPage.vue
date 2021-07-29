<template>
  <div>
    <ProjectCard
      :img="require('@/assets/tower-dropper-screenshot.webp')"
      :video="require('@/assets/tower-dropper-gameplay.mp4')"
      ><h1>Tower Dropper</h1>
      <br />
      <p>
        Tower dropper is a mobile stacking game. The higher you build the tower,
        the more points you get.<br />
        Watch out though, someone keeps loading up the crane with TNT. Who
        thought it would be a good idea to store TNT with the buildings?
        <br /><br />
        Developed in Unity (2020)
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
      :img="require('@/assets/jump-screenshot.png')"
      :video="require('@/assets/jump-gameplay.mp4')"
      ><h1>Jump</h1>
      <br />
      <p>
        Climb your way up higher and higher by launching yourself from wall to
        wall. <br />
        Don't take too long though, if you're too slow the acid will catch up
        and your game will be over.
        <br /><br />
        Developed in Unity (2020)
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
    <ProjectCard
      :img="require('@/assets/pong-screenshot.png')"
      :video="require('@/assets/pong-gameplay.mp4')"
      ><h1>Pong</h1>
      <br />
      <p>
        A basic recreation of the classic Pong game.<br /><br />
        Move your paddle up and down to hit the ball back to the other
        player.<br />
        Angle your return by hitting the ball with the extremes of your
        paddle.<br />
        If the other player misses it, you get a point.
        <br />
        <br />
        Developed in Python 3 with Pygame (2020)
      </p>
      <br />
      <a href="https://github.com/JohnnyHowe/pong" target="_blank"
        ><img
          class="github"
          alt="Check it out on GitHub"
          src="@/assets/github-icon.png"
      /></a>
    </ProjectCard>
    <ProjectCard :img="require('@/assets/raytracer.png')"
      ><h1>OpenGL Raytracer</h1>
      <br />
      <p>
        Simple raytracer able to recursivley trace through solid, transparent,
        refractive, and reflective objects to produce a more realistic scene
        than the OpenGL2 pipeline allows. <br /><br />
        Created in C++ with OpenGL2 (2021)
      </p>
      <br />
      <a href="https://github.com/JohnnyHowe/opengl-raytracer" target="_blank"
        ><img
          class="github"
          alt="Check it out on GitHub"
          src="@/assets/github-icon.png"
      /></a>
    </ProjectCard>
    <ProjectCard
      :img="require('@/assets/opengl-animation-screenshot.png')"
      :video="require('@/assets/opengl-animation.mp4')"
      ><h1>OpenGL Animation</h1>
      <br />
      <p>
        Simple physics based animation.<br/>
        Shows scene containing basic shapes and a sweep surface.
        <br />
        <br />
        Developed in C++ with OpenGL2 (2020)
      </p>
      <br />
      <a href="https://github.com/JohnnyHowe/opengl2-animation" target="_blank"
        ><img
          class="github"
          alt="Check it out on GitHub"
          src="@/assets/github-icon.png"
      /></a>
    </ProjectCard>
    <ProjectCard
      :img="require('@/assets/snake-screenshot.png')"
      :video="require('@/assets/snake-gameplay.mp4')"
      ><h1>Snake</h1>
      <br />
      <p>
        My basic recreation of the classic Snake game.<br /><br />
        Move around with the WASD or arrow keys to navigate to the food.<br />
        Watch out, if you eat your own tail, it's game over.
        <br />
        <br />
        Created with JavaScript and the HTML5 Canvas (2019)
      </p>
      <br />
      <a href="https://github.com/JohnnyHowe/snake-js" target="_blank"
        ><img
          class="github"
          alt="Check it out on GitHub"
          src="@/assets/github-icon.png"
      /></a>
      <a href="https://johnnyhowe.github.io/snake-js/" target="_blank"
        ><img class="github" alt="Play it now" src="@/assets/play-button.png"
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
.github {
  height: min(8vh, 4vw);
  padding: min(2vh, 1vw);
}
</style>