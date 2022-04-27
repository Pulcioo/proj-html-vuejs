<template>
  <div class="img_container d-flex justify-content-center w-100 absolute">
    <div
      v-for="(item, index) in cards"
      :key="index"
      class="d-flex align-items-end m-4"
    >
      <img :src="'images/' + cards[index].url" alt="cover" id="cover" />
      <div class="d-flex flex-column m-3 info">
        <span
          ><i class="fa-solid fa-angle-up"></i
          ><i class="fa-solid fa-angle-up"></i
          ><i class="fa-solid fa-angle-up"></i
        ></span>
        <span>{{ cards[index].title }}</span>
        <span class="yellow small">{{ cards[index].message }}</span>
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
#cover {
  height: 300px;
  width: 280px;
}

.info {
  position: absolute;
}
</style>