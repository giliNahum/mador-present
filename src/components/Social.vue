<template>
  <div id="social">
    <video
      v-for="(video, i) in socialVideos"
      :key="i"
      :src="video"
      class="tiktok"
      controls
      autoplay
      muted
    ></video>
  </div>
</template>

<script>
export default {
  name: "social",
  components: {},
  data() {
    return {
      socialVideos: [
        "./assets/social/jet2.mp4",
        "./assets/social/ztair.mp4",
        "./assets/social/funkyWorld.mp4",
        "./assets/social/familyWeek.mp4",
        "./assets/social/roomTour.mp4",
        "./assets/social/rsarit.mp4",
        "./assets/social/noaKirel.mp4",
        "./assets/social/food.mp4",
        "./assets/social/streetTalk2.mp4",
      ],
    };
  },
  methods: {},
};
</script>

<style scoped>
#social {
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  flex-wrap: wrap;
}

.tiktok {
  margin: 1rem 1rem;
  max-height: 30rem;
}
</style>
