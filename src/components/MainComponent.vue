<template>
  <div class="container-fluid">
    <ShopComponent />
    <CitComponent />
  </div>
</template>

<script>
import ShopComponent from "@/components/ShopComponent.vue";
import CitComponent from "@/components/CitComponent.vue";

export default {
  name: "MainComponent",
  components: {
    ShopComponent,
    CitComponent,
  },
};
</script>

<style scoped lang="scss">
</style>