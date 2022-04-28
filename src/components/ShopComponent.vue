<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-7 offset-1 d-flex align-items-center">
        <div class="container_text">
          <span class="red">Certified fitness professional</span>
          <h1>Take control of your health</h1>
          <span
            ><i class="fa-solid fa-angle-up yellow fa-2x"></i
            ><i class="fa-solid fa-angle-up yellow fa-2x"></i
            ><i class="fa-solid fa-angle-up yellow fa-2x"></i
          ></span>
          <p>
            Curabitur non nulla sit ametnisl tempus convallis quis ac lectus
            dolor sit amet.
          </p>
          <button class="btn btn_blue px-4" id="channel">
            <i class="fa-brands fa-youtube"></i> Visit my YouTube channel
          </button>
          <button class="btn btn_black px-4" id="buy">
            Buy Avada today <i class="fa-solid fa-arrow-right"></i>
          </button>
        </div>
      </div>
      <div class="col-3 d-flex justify-content-center align-items-center">
        <i class="fa-solid fa-circle-play fa-4x"></i>
      </div>
      <div class="col-1 d-flex justify-content-end">
        <div class="p-2">
          <div class="box d-flex justify-content-center mb-1 mt-5">
            <div
              class="
                d-flex
                flex-column
                justify-content-center
                align-items-center
              "
            >
              <span><i class="fa-solid fa-laptop black"></i></span>
              <span id="on-sale">Demos</span>
            </div>
          </div>
          <div class="box d-flex justify-content-center">
            <div
              class="
                d-flex
                flex-column
                justify-content-center
                align-items-center
              "
            >
              <span id="price">$39</span>
              <span id="on-sale">On Sale</span>
            </div>
          </div>
        </div>
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

  .container_text {
    padding-left: 1rem;

    h1 {
      font-size: 50px;
    }

    #channel:hover {
      background-color: red;
      color: white;
    }

    #buy:hover {
      background-color: white;
      color: black;
    }
  }

  .box {
    height: 50px;
    width: 50px;
    background-color: white;
    border-radius: 8px;

    #price {
      color: rgb(38, 169, 38);
    }

    #on-sale {
      font-size: x-small;
      color: #78787a;
    }
  }
}
</style>