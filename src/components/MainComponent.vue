<template>
  <div class="container-fluid">
    <ShopComponent />
    <CitComponent :cards="cards" />
    <YouTubeComponent :playlist="playlist" />
    <EmailComponent />
    <InfoComponent :info="info" />
  </div>
</template>

<script>
import ShopComponent from "@/components/ShopComponent.vue";
import CitComponent from "@/components/CitComponent.vue";
import YouTubeComponent from "@/components/YouTubeComponent.vue";
import EmailComponent from "@/components/EmailComponent.vue";
import InfoComponent from "@/components/InfoComponent.vue";

export default {
  name: "MainComponent",
  components: {
    ShopComponent,
    CitComponent,
    YouTubeComponent,
    EmailComponent,
    InfoComponent,
  },
  props: {
    cards: Array,
    playlist: Array,
    info: Array,
  },
};
</script>

<style scoped lang="scss">
</style>