<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-10 offset-1 d-flex justify-content-between">
        <div v-for="(item, index) in info" :key="index" class="text-center p-3">
          <div class="border py-5">
            <i :class="item.icon" class="py-4"></i>
            <h5 class="d-block">{{ item.title }}</h5>
            <span class="yellow">{{ item.subtitle }}</span>
            <p class="gray small py-4">
              {{ item.message }}
            </p>
            <span class="small">{{ item.message2 }}</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "InfoContainer",
  props: {
    info: Array,
  },
};
</script>

<style scoped lang="scss">
.row {
  padding: 60px 0;

  .border {
    border: 3px solid #4154fe !important;

    &:hover i {
      font-size: 80px;
    }
  }
}
</style>