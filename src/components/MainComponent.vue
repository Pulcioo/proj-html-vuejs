<template>
  <div class="container-fluid">
    <ShopComponent />
  </div>
</template>

<script>
import ShopComponent from "@/components/ShopComponent.vue";

export default {
  name: "MainComponent",
  components: {
    ShopComponent,
  },
};
</script>

<style scoped lang="scss">
</style>