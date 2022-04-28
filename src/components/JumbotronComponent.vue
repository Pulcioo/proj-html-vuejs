<template>
  <div class="container-fluid">
    <div
      class="row d-flex flex-column align-content-center justify-content-center"
    >
      <div class="col-5 text-center">
        <h2>
          "I've failed over and over again in my life. And that is why I
          succeed."
        </h2>
        <span
          ><i class="fa-solid fa-angle-up yellow fa-2x"></i
          ><i class="fa-solid fa-angle-up yellow fa-2x"></i
          ><i class="fa-solid fa-angle-up yellow fa-2x"></i
        ></span>
        <p>
          Arcu auctor gravida nisl, congue sit nisi tincidunt eget proin. In
          lacinia lacus donec sed massa in ipsum eros, tristique. Gravida
          suspendisse etiam in iaculis
        </p>
        <button class="btn btn_blue px-4">Buy Avada today ></button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "JumbotronComponent",
};
</script>

<style scoped lang="scss">
.row {
  background-image: url(@/assets/banner2-2x.jpg);
  background-size: cover;
  height: 500px;
}
</style>