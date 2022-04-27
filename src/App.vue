<template>
  <div id="app">
    <HeaderComponent :menuItem="menuItem" />
    <MainComponent :cards="cards" />
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import MainComponent from "./components/MainComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";

export default {
  name: "App",
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
  },
  data() {
    return {
      menuItem: [
        { message: "Home" },
        { message: "Services" },
        { message: "About" },
        { message: "Videos" },
        { message: "Blog" },
        { message: "Store" },
      ],
      cards: [
        {
          url: "service6-2x.jpg",
          title: "Crossfit workout",
          message: "Push your limits",
        },
        {
          url: "box1-2x.jpg",
          title: "New gym apparel",
          message: "Look good, feel good",
        },
        {
          url: "box3-2x.jpg",
          title: "Team training",
          message: "Find a partner",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "@/style/general";

[class*="col"] {
  border: 1px dashed red;
}
</style>
