<template>
  <div class="container-fluid">
    <div class="video_container d-flex justify-content-center">
      <div v-for="(item, index) in articles" :key="index" class="p-3">
        <div class="d-flex flex-column m-3">
          <div class="wrapper">
            <div class="overlay"></div>
            <img :src="'images/' + item.url" alt="video" id="video" />
          </div>
          <span class="mt-3 black mx-2">{{ item.title }}</span>
          <span class="small gray mx-2">{{ item.message }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ArticleItem",
  props: {
    articles: Array,
  },
};
</script>

<style scoped lang="scss">
.wrapper {
  position: relative;

  .overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 200px;

    &:hover {
      background-image: linear-gradient(transparent, rgba(27, 97, 226, 0.5));
    }
  }
}

#video {
  height: 200px;
  width: 100%;
  border-radius: 5px;
  border-bottom-right-radius: 25px;
}
</style>