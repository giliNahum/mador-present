<template>
    <div id="campus">
      <video
        src=""
        class="video"
        controls
        autoplay
        muted
      ></video>
    </div>
  </template>
  
  <script>
  export default {
    name: "campus",
    components: {},
    data() {
      return {
        socialVideos: [
        ],
      };
    },
    methods: {},
  };
  </script>
  
  <style scoped>
  #campus {
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    flex-wrap: wrap;
  }
  
  .video {
    margin: 1rem 1rem;
    max-height: 30rem;
  }
  </style>