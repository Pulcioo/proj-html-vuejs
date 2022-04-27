<template>
  <div class="container-fluid">
    <ShopComponent />
    <CitComponent :cards="cards" />
    <YouTubeComponent :playlist="playlist" />
    <EmailComponent />
    <InfoComponent :info="info" />
    <ArticlesComponent :articles="articles" />
  </div>
</template>

<script>
import ShopComponent from "@/components/ShopComponent.vue";
import CitComponent from "@/components/CitComponent.vue";
import YouTubeComponent from "@/components/YouTubeComponent.vue";
import EmailComponent from "@/components/EmailComponent.vue";
import InfoComponent from "@/components/InfoComponent.vue";
import ArticlesComponent from "@/components/ArticlesComponent.vue";

export default {
  name: "MainComponent",
  components: {
    ShopComponent,
    CitComponent,
    YouTubeComponent,
    EmailComponent,
    InfoComponent,
    ArticlesComponent,
  },
  props: {
    cards: Array,
    playlist: Array,
    info: Array,
    articles: Array,
  },
};
</script>

<style scoped lang="scss">
</style>