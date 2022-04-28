<template>
  <div class="video_container d-flex justify-content-center">
    <div v-for="(item, index) in playlist" :key="index" class="p-3">
      <div class="d-flex flex-column m-3">
        <div class="wrapper">
          <div class="icon d-flex justify-content-center align-items-center">
            <i class="fa-solid fa-circle-play 4x"> </i>
          </div>
          <img :src="'images/' + item.url" alt="video" id="video" />
        </div>
        <span class="text-center mt-3">{{ item.title }}</span>
        <span class="text-center small blue">{{ item.message }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "VideoItem",
  props: {
    playlist: Array,
  },
};
</script>

<style scoped lang="scss">
.wrapper {
  position: relative;

  .icon {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 200px;

    i {
      color: white;
      font-size: xx-large;
    }

    &:hover i {
      font-size: 60px;
      color: red;
    }
  }

  #video {
    height: 200px;
    width: 100%;
    border-radius: 5px;
    border-bottom-right-radius: 25px;
  }
}
</style>