<template>
  <div class="container-fluid white">
    <div class="black">
      <div class="col-10 offset-1 d-flex">
        <div
          v-for="(item, index) in clubs"
          :key="index"
          class="d-flex flex-column align-items-center text-center p_90"
        >
          <img :src="'images/' + item.url" alt="logo" />
          <span
            ><i class="fa-solid fa-angle-up blue"></i
            ><i class="fa-solid fa-angle-up blue"></i
            ><i class="fa-solid fa-angle-up blue"></i
          ></span>
          <p class="small gray">{{ item.message }}</p>
          <span class="small">{{ item.subtitle }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FitnessComponent",
  props: {
    clubs: Array,
  },
};
</script>

<style scoped lang="scss">
img {
  width: 120px;
}
</style>