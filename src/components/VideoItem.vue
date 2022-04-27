<template>
  <div class="video_container d-flex justify-content-center">
    <div v-for="(item, index) in playlist" :key="index" class="p-3">
      <div class="d-flex flex-column m-3">
        <img :src="'images/' + item.url" alt="video" id="video" />
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
#video {
  height: 200px;
  width: 300px;
  border-radius: 5px;
  border-bottom-right-radius: 25px;
}
</style>