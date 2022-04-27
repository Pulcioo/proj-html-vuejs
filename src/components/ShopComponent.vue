<template>
  <div class="row">
    <div class="col-7 offset-1 d-flex align-items-center">
      <div class="container_text">
        <span class="red">Certified fitness professional</span>
        <h1>Take control of your health</h1>
        <p>
          Curabitur non nulla sit ametnisl tempus convallis quis ac lectus dolor
          sit amet.
        </p>
        <button class="btn btn_blue px-4">
          <i class="fa-brands fa-youtube"></i> Visit my YouTube channel
        </button>
        <button class="btn btn_black px-4">
          Buy Avada today <i class="fa-solid fa-arrow-right"></i>
        </button>
      </div>
    </div>
    <div class="col-3 d-flex justify-content-center align-items-center">
      <i class="fa-solid fa-circle-play fa-2xl"></i>
    </div>
    <div class="col-1 d-flex justify-content-end">
      <div>
        <div class="box mb-1 mt-5"></div>
        <div class="box"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ShopComponent",
};
</script>

<style scoped lang="scss">
.row {
  background-image: url(@/assets/slider82x-scaled.jpg);
  background-size: cover;
  height: 500px;

  h1 {
    font-size: 50px;
  }

  .box {
    height: 50px;
    width: 50px;
    background-color: white;
  }
}
</style>