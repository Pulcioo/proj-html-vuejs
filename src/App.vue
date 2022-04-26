<template>
  <div id="app">
    <HeaderComponent :menuItem="menuItem" />
    <MainComponent />
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
