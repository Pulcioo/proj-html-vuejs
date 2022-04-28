<template>
  <div id="app">
    <HeaderComponent :menuItem="menuItem" />
    <MainComponent
      :cards="cards"
      :playlist="playlist"
      :info="info"
      :articles="articles"
      :clubs="clubs"
    />
    <FooterComponent :footerItem="footerItem" />
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
      playlist: [
        {
          url: "video2-2x.jpg",
          title: "Thighs e glute workout",
          message: "Increase your mobility",
        },
        {
          url: "video7-2x.jpg",
          title: "Lift, firm e perk up",
          message: "Feel young again",
        },
        {
          url: "video9-2x.jpg",
          title: "Slim e trim your waist",
          message: "Shed those extra pounds",
        },
      ],
      info: [
        {
          icon: "fa-solid fa-stopwatch fa-3x",
          title: "Thighs e glute workout",
          subtitle: "Find a partner",
          message:
            "Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senectus aget sed duis veicula.",
          message2: "Find a patner >",
        },
        {
          icon: "fa-solid fa-heart-pulse fa-3x",
          title: "Crossfit workout",
          subtitle: "Push your limit",
          message:
            "Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senectus aget sed duis veicula.",
          message2: "Learn about Crossfit >",
        },
        {
          icon: "fa-solid fa-child-reaching fa-3x",
          title: "Weight loss plan",
          subtitle: "Shed those pounds",
          message:
            "Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senectus aget sed duis veicula.",
          message2: "Schedule a workout >",
        },
      ],
      articles: [
        {
          url: "blog4-2x.jpg",
          title: "The best proteine shake",
          message: "By Admin | November 26th, 2019 | Gym",
        },
        {
          url: "blog3-2x.jpg",
          title: "Ultimate cardio workout",
          message: "By Admin | November 26th, 2019 | Gym",
        },
        {
          url: "blog1-2x.jpg",
          title: "New juices available now",
          message: "By Admin | November 26th, 2019 | Gym",
        },
      ],
      clubs: [
        {
          url: "sponsor-1-2x-200x103.png",
          message:
            "Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senectus aget sed duis veicula.",
          subtitle: "Visit Yoga Studio >",
        },
        {
          url: "sponsor-2-2x-200x103.png",
          message:
            "Feugiat ediam ui mauis pharetra mauris sed pharetra. Convallis sapien ornare cras faucibus nulla porta dui a.",
          subtitle: "Join Fitness Center >",
        },
        {
          url: "sponsor-3-2x-200x103.png",
          message:
            "Nisi at quas adisciping montes, nec, adipiscing commodo aquilam tincidut. Ligula in habitant et saggittis imperdient.",
          subtitle: "Learn about FC >",
        },
        {
          url: "sponsor-4-2x-200x103.png",
          message:
            "Proin in viverra maecenas es mattis ut hib enim. Gravida ultricies mi porta lacus. Et psuere velitsec net elefeind.",
          subtitle: "Visit Power Gym >",
        },
      ],
      footerItem: [
        { message: "> The best protein shake" },
        { message: "> Ultimate cardio workout" },
        { message: "> New juices available now" },
        { message: "> Tips to find training partners" },
        { message: "> 20 best healty recipes" },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "@/style/general";

// [class*="col"] {
// border: 1px dashed red;
// }
</style>
