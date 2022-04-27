<template>
  <div class="container-fluid">
    <ShopComponent />
    <CitComponent :cards="cards" />
    <YouTubeComponent :playlist="playlist" />
    <EmailComponent />
  </div>
</template>

<script>
import ShopComponent from "@/components/ShopComponent.vue";
import CitComponent from "@/components/CitComponent.vue";
import YouTubeComponent from "@/components/YouTubeComponent.vue";
import EmailComponent from "@/components/EmailComponent.vue";

export default {
  name: "MainComponent",
  components: {
    ShopComponent,
    CitComponent,
    YouTubeComponent,
    EmailComponent,
  },
  props: {
    cards: Array,
    playlist: Array,
  },
};
</script>

<style scoped lang="scss">
</style>