<template>
  <div class="article">
    <div class="inner-article">
      <article-cards/>
    </div>
  </div>
</template>

<script>
import ArticleCards from '@/components/ArticleCards.vue'
export default {
  components: { ArticleCards },

}
</script>

<style>
.article{
    width: 100%;
    height: 1073px;
      background-image: url('/bg@2x.png');
  background-size:cover ;
    display: block;
    
}
.inner-article{
  padding-top: 126px;
  display: block;
  margin: auto;

  height: 100%;
}
@media screen and (max-width: 1180px) {
  .article{
    height: auto;
  }
}

</style>