<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col">
        <div class="block w-100 h-100">
          <div
            class="
              content
              d-flex
              flex-column
              justify-content-center
              align-items-center
            "
          >
            <i class="fa-solid fa-circle-play fa-4x p-3"></i>
            <h2>Crossfit workout of the day</h2>
            <h3 class="yellow">November 15th, 2019</h3>
            <span>View all videos <i class="fa-solid fa-arrow-right"></i></span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SecondJumbotron",
};
</script>

<style scoped lang="scss">
.row {
  height: 500px;

  .block {
    position: relative;
    background: url(@/assets/banner14-2x.jpg);
    background-size: cover;

    .content {
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: linear-gradient(to left top, red, blue);
      opacity: 0.7;
      padding: 10px;
    }
  }
}
</style>