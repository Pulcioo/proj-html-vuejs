<template>
  <div class="container-fluid white">
    <div class="row relative">
      <div class="col">
        <div
          id="workout"
          class="d-flex justify-content-center align-items-center"
        >
          <i class="fa-solid fa-circle-play fa-4x"></i>
        </div>
      </div>
      <div class="col black">
        <div class="p_100">
          <span class="blue">Tune up your workouts</span>
          <h2 class="mt-4 mb-4">The best health & fitness advice online</h2>
          <div class="d-flex pb_20">
            <img src="images/unnamed.jpg" alt="logo" id="logo" />
            <div class="d-flex flex-column">
              <span class="x_small gray">Theme Fusion</span>
              <div id="yt-block" class="x_small d-flex align-items-center">
                <div id="mini_block">
                  <i class="fa-brands fa-youtube"></i> YouTube
                </div>
                <div id="followers">
                  <span class="gray">999+</span>
                </div>
              </div>
            </div>
          </div>
          <p class="gray mb-4">
            Arcu eu facilisi ut quisque placerat nunc habitant. Magna semper
            mauris, venenatis, leo integer sit pellentesque.
          </p>
          <button class="btn btn_red px-4">
            <i class="fa-brands fa-youtube"></i> Visit my YouTube channel
          </button>
        </div>
      </div>
    </div>
    <div class="row d-flex flex-column black">
      <div class="col-10 offset-1 d-flex justify-content-between mt-100">
        <span>Featured playlist</span>
        <span class="small">View all videos ></span>
      </div>
      <div class="col">
        <VideoItem :playlist="playlist" />
      </div>
    </div>
  </div>
</template>

<script>
import VideoItem from "@/components/VideoItem.vue";

export default {
  name: "YouTubeComponent",
  props: {
    playlist: Array,
  },
  components: {
    VideoItem,
  },
};
</script>

<style scoped lang="scss">
#workout {
  background-image: url(@/assets/service15-2x.jpg);
  background-size: cover;
  height: 500px;
  width: 50%;
  border-bottom-right-radius: 25px;
  position: absolute;
  bottom: 50px;
}

#logo {
  width: 40px;
  padding-right: 5px;
}

#yt-block {
  border: 1px gray solid;

  #mini_block {
    background-color: red;
    color: white;
    padding: 0 4px;
  }

  #followers {
    padding: 0 4px;
  }
}
</style>