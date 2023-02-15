<template>
  <div>
<cover/>
<article-zone/>
<channel/>
<footer-zone/>
  </div>
</template>

<script>
import Cover from '@/components/Cover.vue'
import ArticleZone from '@/components/ArticleZone.vue'
import FooterZone from '@/components/FooterZone.vue'
import Channel from '@/components/Channel.vue'
export default {
  components: { Cover,ArticleZone,FooterZone,Channel },
  name: 'IndexPage'
}
</script>


<style>
*{
  padding: 0;
  margin: 0;
  font-family: 'Tahoma',sans-serif;
  font-size: 15px;
  box-sizing: border-box;
}
body{
  overflow-x: hidden;
  width: 100%;
}


.responsive_scope{
  max-width: 1170px;
}

@media screen and (max-width:1180px){
    .responsive_scope{
      width: 100%;
      
      padding: 0px 20px 0px 20px;
    }
}
</style>