<template>
  <div class="container-fluid white">
    <div
      class="
        text-container
        col-10
        offset-1
        d-flex
        justify-content-between
        black
      "
    >
      <span>Latest articles</span>
      <span class="small">Read all articles ></span>
    </div>
    <div class="col">
      <ArticleItem :articles="articles" />
    </div>
  </div>
</template>

<script>
import ArticleItem from "@/components/ArticleItem.vue";

export default {
  nome: "ArticlesComponent",
  props: {
    articles: Array,
  },
  components: {
    ArticleItem,
  },
};
</script>

<style scoped lang="scss">
.text-container {
  padding-top: 100px;
}
</style>