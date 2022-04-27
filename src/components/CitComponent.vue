<template>
  <div class="gradient relative">
    <div class="row flex-column">
      <div class="col">
        <div class="img_container d-flex justify-content-center absolute">
          <div id="image-1" class="d-flex align-items-end m-3">
            <div class="d-flex flex-column m-3">
              <span>Crossfit workout</span>
              <span class="yellow small">Push your limits</span>
            </div>
          </div>
          <div id="image-2" class="d-flex align-items-end m-3">
            <div class="d-flex flex-column m-3">
              <span>New gym apparel</span>
              <span class="yellow small">Look good, feel good</span>
            </div>
          </div>
          <div id="image-3" class="d-flex align-items-end m-3">
            <div class="d-flex flex-column m-3">
              <span>Crossfit workout</span>
              <span class="yellow small">Push your limits</span>
            </div>
          </div>
        </div>
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
          <div>
            <img
              src="@/assets/images/avatar-1-2x.jpg"
              alt="profile"
              id="img_profile"
            />
            <span class="p-2">Brad Johnson</span>
            <span class="gray">Las Vegas</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CitComponent",
};
</script>

<style scoped lang="scss">
.gradient {
  background: linear-gradient(to left top, red, blue);

  #image-1 {
    background-image: url(@/assets/images/service6-2x.jpg);
    background-size: cover;
    height: 250px;
    width: 220px;
  }

  #image-2 {
    background-image: url(@/assets/images/box1-2x.jpg);
    background-size: cover;
    height: 250px;
    width: 220px;
  }

  #image-3 {
    background-image: url(@/assets/images/box3-2x.jpg);
    background-size: cover;
    height: 250px;
    width: 220px;
  }

  .text_container {
    margin-top: 270px;
    margin-bottom: 100px;

    p {
      font-size: 20px;
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