<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-10 offset-1 d-flex justify-content-between">
        <div v-for="(item, index) in info" :key="index" class="text-center p-3">
          <div class="border py-5">
            <i :class="info[index].icon" class="py-4"></i>
            <h5 class="d-block">{{ info[index].title }}</h5>
            <span class="yellow">{{ info[index].subtitle }}</span>
            <p class="gray small py-4">
              {{ info[index].message }}
            </p>
            <span class="small">{{ info[index].message2 }}</span>
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
  }
}
</style>