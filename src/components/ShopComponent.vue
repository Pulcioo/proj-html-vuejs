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
        <button class="btn btn_blue px-4">Schedule a workout</button>
        <button class="btn btn_black px-4">Schedule a workout</button>
      </div>
    </div>
    <div class="col-3 d-flex justify-content-center align-items-center">
      <i class="fa-solid fa-circle-play fa-2xl"></i>
    </div>
    <div class="col-1"></div>
  </div>
</template>

<script>
export default {
  name: "ShopComponent",
};
</script>

<style scoped lang="scss">
.row {
  background-image: url(@/assets/images/slider82x-scaled.jpg);
  background-size: cover;
  height: 450px;

  h1 {
    font-size: 50px;
  }
}

// utilities
.red {
  color: red;
}

.btn_blue {
  background-color: #4154fe;
  color: white;
  border-radius: 50px;
}

.btn_black {
  background-color: black;
  color: white;
  border-color: gray;
  border-radius: 50px;
  margin-left: 10px;
}
</style>