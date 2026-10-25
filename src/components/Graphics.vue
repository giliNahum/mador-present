<template>
  <div id="graphics">
    <video
      v-for="(video, i) in videoData"
      :key="i"
      :src="video"
      class="video"
      controls
      autoplay
      muted
    ></video>
    <img
      v-for="(graphic, i) in data"
      :key="i"
      :src="graphic"
      :alt="'graphic'"
      class="graphic"
    />
  </div>
</template>

<script>
export default {
  name: "graphics",
  components: {},
  data() {
    return {
      data: [
        "./assets/graphics/soacialLogo.png",
        "./assets/graphics/rollup.png",
        "./assets/graphics/videoCourse.png",
        "./assets/graphics/alergens.png",
        "./assets/graphics/didYouKnow.png",
        "./assets/graphics/boded.jpg",
        "./assets/graphics/magal1.png",
        "./assets/graphics/magal2.png",
        "./assets/graphics/vip1.png",
        "./assets/graphics/vip2.png",
        "./assets/graphics/hokara.png",
        "./assets/graphics/yzTamuz.jpg",
        "./assets/graphics/log.jpg",
        "./assets/graphics/sganim2.png",
        "./assets/graphics/sganim1.jpeg",
        "./assets/graphics/arrest1.png",
        "./assets/graphics/arrest4.png",
        "./assets/graphics/arrest2.png",
        "./assets/graphics/arrest3.png",
        "./assets/graphics/cranes1.png",
        "./assets/graphics/cranes2.png",
        "./assets/graphics/cranes3.png",
        "./assets/graphics/cranes4.png",
        "./assets/graphics/hadmaya1.png",
        "./assets/graphics/synagogue.png",
      ],
      videoData: [
        "./assets/graphics/socialAnimation.mp4",
      ],
    };
  },
  methods: {},
};
</script>

<style scoped>
#graphics {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-content: center;
}

.graphic {
  max-width: 52rem;
  max-height: 25rem;
  margin: 0.5rem 0.5rem;
}

.video {
  margin: 1rem 1rem;
  height: 25rem;
}
</style>
