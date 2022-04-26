<template>
  <div class="container">
    <div class="row">
      <div class="col">
        <img src="@/assets/images/logo.png" alt="" />
      </div>
      <div class="col-6 d-flex align-items-center">
        <ul class="d-flex w-100 justify-content-around mb-0">
          <li v-for="item in menuItem" :key="item.message">
            <a href="#">{{ item.message }}</a>
          </li>
        </ul>
      </div>
      <div class="col">
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

    a {
      text-decoration: none;
      color: #78787a;

      &:hover {
        color: white;
      }
    }
  }
}

.btn_blue {
  background-color: #4154fe;
  color: white;
  border-radius: 50px;
}
</style>