<template>
  <div class="container-fluid">
    <div class="row d-flex justify-content-center text-center" id="footer">
      <div class="col d-flex flex-column align-items-center px-5">
        <img src="images/logo.png" alt="logo" />
        <p class="gray small">
          Ac aliquam nege saggittis dia faucibus vitae purus turpis phasellus.
          Pellentesque consecteur amet purus ultrices mauris.
        </p>
        <div>
          <i class="fa-brands fa-facebook-f m-2 red"></i>
          <i class="fa-brands fa-twitter m-2 red"></i>
          <i class="fa-brands fa-youtube m-2 red"></i>
          <i class="fa-brands fa-instagram m-2 red"></i>
          <i class="fa-brands fa-linkedin-in m-2 red"></i>
        </div>
      </div>
      <div class="col">
        <ul>
          <span>RECENT POSTS</span>
          <li v-for="item in footerItem" :key="item.message">
            <a href="#" class="small">{{ item.message }}</a>
          </li>
        </ul>
      </div>
      <div class="col">
        <div class="info-text">
          <span>CONTACT INFORMATIONS</span>
          <p class="gray small">4746 Tipple Road Michigan 48449</p>
          <div class="d-flex flex-column">
            <span class="small">Mobile: 1.800.000.0000</span>
            <span class="small">Email: info@your-company.com</span>
          </div>
        </div>
      </div>
    </div>
    <div class="row">
      <hr />
      <p class="gray py-3 text-center" id="pie">
        © Copyright 2012 - 2020|Avada theme by <span>Theme Fusion</span>|All
        rights reserved|Powered By <span>WordPress</span>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterComponent",
  props: {
    footerItem: Array,
  },
};
</script>

<style scoped lang="scss">
#footer {
  padding: 90px 180px;

  img {
    width: 180px;
    padding-bottom: 10px;
  }

  ul {
    line-height: 30px;

    li {
      list-style-type: none;

      a {
        text-decoration: none;
        color: white;

        &:hover {
          color: red;
        }
      }
    }
  }

  .info-text p {
    padding: 15px;
  }
}

#pie {
  font-size: 12px;

  span {
    color: white;
  }
}
</style>