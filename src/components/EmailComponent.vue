<template>
  <div class="container-fluid">
    <div class="row d-flex flex-column">
      <div class="col-10 offset-1 mb-2">
        <span class="red">Join our mailing list today</span>
      </div>
      <div class="col-5 offset-1">
        <h2>Insider offers & flash sales in your inbox every week.</h2>
      </div>
      <div class="col-10 offset-1 mt-2 mb-4">
        <i class="fa-solid fa-angle-up yellow"></i>
        <i class="fa-solid fa-angle-up yellow"></i>
        <i class="fa-solid fa-angle-up yellow"></i>
      </div>
      <div class="col-10 offset-1">
        <div class="mb-3">
          <input
            type="email"
            class="form-control d-inline w_35"
            placeholder="Insert your email...*"
          />
          <button class="btn btn_blue px-5 ml-30">Subscribe</button>
        </div>
      </div>
      <div class="col-5 offset-1">
        <p class="gray small">
          Curabitur non nulla sit amet nisl tempus convallis quis ac lectus
          dolor sit amet, consectetur adipiscing elit sed portittor lectus.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "EmailComponent",
};
</script>

<style scoped lang="scss">
.row {
  padding: 100px 0;
  background-image: url(@/assets/banner1-2x.jpg);
  background-size: cover;

  input {
    border-radius: 20px;
  }
}
</style>