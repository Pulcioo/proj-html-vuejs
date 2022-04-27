<template>
  <div class="gradient relative">
    <div class="row">
      <div class="col">
        <CardItem :cards="cards" />
      </div>
    </div>
    <div class="row d-flex justify-content-center">
      <div class="col-5">
        <div class="text_container text-center">
          <p>
            "How do you responde to the challenge in the second half will
            determine what you become after the game, whether you are winner or
            a loser."
          </p>
          <span
            ><i class="fa-solid fa-angle-up yellow fa-2x"></i
            ><i class="fa-solid fa-angle-up yellow fa-2x"></i
            ><i class="fa-solid fa-angle-up yellow fa-2x"></i
          ></span>
          <div>
            <img src="images/avatar-1-2x.jpg" alt="profile" id="img_profile" />
            <span class="p-2">Brad Johnson</span>
            <span class="gray">Las Vegas</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CardItem from "@/components/CardItem.vue";

export default {
  name: "CitComponent",
  props: {
    cards: Array,
  },
  components: {
    CardItem,
  },
};
</script>

<style scoped lang="scss">
.gradient {
  background: linear-gradient(to left top, red, blue);

  .text_container {
    margin-top: 330px;
    margin-bottom: 140px;

    p {
      font-size: 25px;
    }

    #img_profile {
      width: 30px;
      border-radius: 50%;
      display: inline;
    }

    span {
      font-size: small;
    }
  }
}
</style>