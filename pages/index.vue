<template>
  <div >
<cover/>
<article-zone/>
<channel/>
  <div class="nav_kkp responsive_scope" style="margin:69px auto 26px auto;">
        <h1></h1>
        <button>
          ดูทั้งหมด <span> <i class="fa-solid fa-chevron-right"></i></span>
        </button>
      </div>
<clips/>
<footer-zone/>
  </div>
</template>

<script>
import Cover from '@/components/Cover.vue'
import ArticleZone from '@/components/ArticleZone.vue'
import FooterZone from '@/components/FooterZone.vue'
import Channel from '@/components/Channel.vue'
import Clips from '@/components/Clips.vue'
export default {
  components: { Cover,ArticleZone,FooterZone,Channel,Clips },
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
html{
  width: 100%;
 overflow-x: hidden !important;
}
body{
  overflow-x: hidden !important;
  width: 100%;
}

.nav_kkp{
  width: 100%;
  height: 40px;
  overflow: hidden;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  margin-bottom: 26px;
}
.nav_kkp h1{
    font-family: 'Kanit',sans-serif;
  font-size: 32px;
  font-weight: 500;
  line-height: 1.25;
  color: #594f74;
}
.nav_kkp button{
    font-family: 'Tahoma',sans-serif;
  font-size: 16px;
  line-height: 1.5;
  color: #84848f;
  background: none;
  border: none;
  padding-top: 10px;
}
.nav_kkp span{
    width: 28px;
  height: 28px;
  display: inline-block;
  margin: 0 0 0 4px;
  object-fit: contain;
  border: 1px solid#dcdcdc;
  border-radius: 50%;
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