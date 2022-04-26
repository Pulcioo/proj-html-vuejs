<template>
  <div class="container">
    <div class="row">
      <div class="col-2 offset-1">
        <img src="@/assets/images/logo.png" alt="" class="w_200" />
      </div>
      <div class="col-5 d-flex align-items-center">
        <ul class="d-flex w-100 justify-content-around mb-0">
          <li v-for="item in menuItem" :key="item.message">
            <a href="#">{{ item.message }}</a>
          </li>
        </ul>
      </div>
      <div class="col-3">
        <div class="d-flex justify-content-end align-items-center">
          <button class="btn btn_blue px-4">Schedule a workout</button>
          <i class="fa-solid fa-cart-shopping mx-4"></i>
          <i class="fa-solid fa-magnifying-glass"></i>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderComponent",
  props: {
    menuItem: Array,
  },
};
</script>

<style scoped lang="scss">
ul {
  padding-left: 5rem;

  li {
    list-style-type: none;
    font-size: 16px;

    a {
      text-decoration: none;
      color: #78787a;

      &:hover {
        color: white;
      }
    }
  }
}

button {
  font-size: 16px;
}

// utilities
.btn_blue {
  background-color: #4154fe;
  color: white;
  border-radius: 50px;
}

.w_200 {
  width: 200px;
}
</style>