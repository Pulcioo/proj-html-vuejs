<template>
  <div class="container-fluid">
    <ShopComponent />
    <CitComponent :cards="cards" />
    <YouTubeComponent :playlist="playlist" />
    <EmailComponent />
    <InfoComponent :info="info" />
    <ArticlesComponent :articles="articles" />
    <JumbotronComponent />
    <FitnessComponent :clubs="clubs" />
  </div>
</template>

<script>
import ShopComponent from "@/components/ShopComponent.vue";
import CitComponent from "@/components/CitComponent.vue";
import YouTubeComponent from "@/components/YouTubeComponent.vue";
import EmailComponent from "@/components/EmailComponent.vue";
import InfoComponent from "@/components/InfoComponent.vue";
import ArticlesComponent from "@/components/ArticlesComponent.vue";
import JumbotronComponent from "@/components/JumbotronComponent.vue";
import FitnessComponent from "@/components/FitnessComponent.vue";

export default {
  name: "MainComponent",
  components: {
    ShopComponent,
    CitComponent,
    YouTubeComponent,
    EmailComponent,
    InfoComponent,
    ArticlesComponent,
    JumbotronComponent,
    FitnessComponent,
  },
  props: {
    cards: Array,
    playlist: Array,
    info: Array,
    articles: Array,
    clubs: Array,
  },
};
</script>

<style scoped lang="scss">
</style>