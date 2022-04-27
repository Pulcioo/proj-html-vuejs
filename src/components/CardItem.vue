<template>
  <div class="img_container d-flex absolute">
    <div
      v-for="(item, index) in cards"
      :key="index"
      class="d-flex align-items-end m-3"
    >
      <img :src="'images/' + cards[index].url" alt="cover" id="cover" />
      <div class="d-flex flex-column m-3 info">
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
  height: 250px;
  width: 230px;
}

.info {
  position: absolute;
}
</style>