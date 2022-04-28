<template>
  <div class="img_container d-flex justify-content-center w-100 absolute">
    <div
      v-for="(item, index) in cards"
      :key="index"
      class="d-flex align-items-end m-4"
    >
      <div class="wrapper">
        <div class="overlay"></div>
        <img :src="'images/' + item.url" alt="cover" id="cover" />
      </div>
      <div class="d-flex flex-column m-3 info">
        <span
          ><i class="fa-solid fa-angle-up"></i
          ><i class="fa-solid fa-angle-up"></i
          ><i class="fa-solid fa-angle-up"></i
        ></span>
        <span>{{ item.title }}</span>
        <span class="yellow small">{{ item.message }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardItem",
  props: {
    cards: Array,
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
    height: 300px;
    background-image: linear-gradient(transparent, rgba(0, 0, 0, 0.4));

    &:hover {
      background-image: linear-gradient(transparent, rgba(0, 0, 0, 0.8));
    }
  }
}

#cover {
  height: 300px;
  width: 100%;
}

.info {
  position: absolute;
}
</style>