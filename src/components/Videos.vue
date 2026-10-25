<template>
  <div id="videos">
    <div v-for="(video, i) in moreVideos" :key="i">
      <video  :src="video.src" class="video" controls></video>
      <p class="video-text">{{ video.text }}</p>
    </div>
  </div>
</template>

<script>
import Carousel from "@/components/Carousel.vue";
export default {
  name: "videos",
  components: {
    Carousel
  },
  data() {
    return {
      gsharimVideos: [
        "./assets/video/gsharim/integration.mp4",
        "./assets/video/gsharim/homeLife.mp4",
        "./assets/video/gsharim/involvement.mp4",
        "./assets/video/gsharim/socialChallenges.mp4",
        "./assets/video/gsharim/statehood.mp4",
      ],
      moreVideos: [
        {src: "./assets/video/acatal.mp4", text: 'יום אנשים - אכאט"ל'},
        {src: "./assets/video/binat.mp4", text: "סרטון תדמית בינת"},
        {src: "./assets/video/dayEran.mp4", text: 'יום בחיי ערן - פרידה ממפקד ק"ה'},
        {src: "./assets/video/fireSafety.mp4", text: 'תרגיל בטיחות בחומ"ס ובאש'},
        {src: "./assets/video/hadracha.mp4", text: 'סיכום עשיית ענף הדרכה במבצע עם כלביא'},
        {src: "./assets/video/medicSayGoodbye.mp4", text: 'סרטון פרידה מראש אט"ל'},
        {src: "./assets/video/randomVideo.mp4", text: "סרטון לטקס חיול - גיבורים קטנים"},
        {src: "./assets/video/releaseVideo.mp4", text: "סרטון ערב פרידה מאנשי מפקדה"},
        {src: "./assets/video/gsharim/integration.mp4", text: 'קורס גשרים - קשיי השתלבות'},
        {src: "./assets/video/gsharim/homeLife.mp4", text: 'קורס גשרים - התנהלות חיי דירה'},
        {src: "./assets/video/gsharim/involvement.mp4", text: 'קורס גשרים - רתימה'},
        {src: "./assets/video/gsharim/socialChallenges.mp4", text: 'קורס גשרים - אתגרים חברתיים'},
        {src: "./assets/video/gsharim/statehood.mp4", text: 'קורס גשרים - ממלכתיות'},
        {src: "./assets/video/kabatim/kabatim1.mp4", text: 'קורס קב"טים - רכב מגיע לש.ג הנהג בורח'},
        {src: "./assets/video/kabatim/kabatim2.mp4", text: 'קורס קב"טים - חטיפת מאבטח'},
        {src: "./assets/video/kabatim/kabatim3.mp4", text: 'קורס קב"טים - אדם מסרב להזדהות'},
        {src: "./assets/video/kabatim/kabatim4.mp4", text: 'קורס קב"טים - פריצה מהגדר'},
        {src: "./assets/video/kabatim/kabatim6.mp4", text: 'קורס קב"טים - חדירת מחבלים לחד"א'},
        {src: "./assets/video/kabatim/kabatim7.mp4", text: 'קורס קב"טים - רחפן עויין מעל הבסיס'},
      ]
    };
  },
  methods: {},
};
</script>

<style scoped>
.carousel-text {
  color: #EDFAFF;
  font-family: "carmela";
  font-size: 1.5rem;
}
#videos {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
  text-align: center;
}

.carousel {
  margin: 0rem 1rem;
}

.video {
  margin: 0rem 1rem;
  width: 40rem;
}

.video-text {
  color: #EDFAFF;
  font-family: "carmela";
  font-size: 1.5rem;
}
</style>
