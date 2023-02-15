<template>
  <div class="article-card-layout">
    <div class="article-zone">
      <div class="article-zone-higlight a1 a2 a3">
        <div class="article-zone-higlight-cover c1 c2 c3">
          <img src="/article/img-article-1.png" alt="" srcset="" />
        </div>
        <div class="article-zone-higlight-detail detail_control">
          <a href="#">
            Margin of Safety กลยุทธ์การลงทุนอย่างปลอดภัย หลักการลงทุนของเบนจามิน
            เกรแฮม
          </a>
          <p>
            ตอบคำถามที่ว่า คุณมีความจำเป็น พร้อมเป็นเจ้าของหรือยัง เช่น
            เพื่อหน้าที่การงาน อาชีพ หรือการเดินทาง ความสะดวกสบาย
            เพราะการซื้อรถนอกจากค่ารถแล้ว ยังมีค่าน้ำมัน ค่าบำรุงรักษา
            ค่าประกันภัย ซึ่งเป็นค่าใช้จ่ายในระยะยาว
          </p>
          <span>การลงทุน</span>
        </div>
      </div>

      <div class="sub-zone e1 e2 e3">
        <div class="article-zone-column b1 b2 b3">
          <div class="article-zone-column-cover d1 d2 d3">
            <img src="/article/img-article-2.png" alt="" srcset="" />
          </div>
          <div class="article-zone-column-detail detail_control">
            <a href="#">
              จับจังหวะการลงทุนเป็นก็สร้างเงินล้านได้ง่ายๆใกล้แค่เอื้อม
            </a>

            <span>การลงทุน</span>
          </div>
        </div>
        <div class="article-zone-column b1 b2 b3">
          <div class="article-zone-column-cover d1 d2 d3">
            <img src="/article/img-article-3.png" alt="" srcset="" />
          </div>
          <div class="article-zone-column-detail detail_control">
            <a href="#">
              Margin of Safety กลยุทธ์การลงทุนอย่างปลอดภัย Margin of Safety
            </a>
            <span>การลงทุน</span>
          </div>
        </div>
      </div>
    </div>
    <div class="gadget-zone r1 r2 r3">
      <div class="side-slide or1 or2">
        <side-slide/>
      </div>
      <div class="side-iframe or1 or2">
        <set-index/>
      </div>
    </div>
  </div>
</template>

<script>
import SideSlide from '@/components/SideSlide'
import SetIndex from '@/components/SetIndex.vue';
export default {
    components:{
        SideSlide,
        SetIndex
    }
};
</script>

<style>
.article-card-layout {
  background: fff;
  width: 100%;
  height: 814px;
  width: 100%;
  max-width: 1170px;
  margin: auto;
  display: flex;
  flex-direction: row;
}
.article-zone {
  width: 100%;
  height: 800px;
}
.article-zone img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.gadget-zone {
  width: 364px;
  height: 800px;
  margin-left: 4px;
  flex-shrink: 0;
}
.side-slide {
  height: 362px;
  width: 100%;
}
.side-iframe {
  width: 100%;
  background: #fff;
  height: 368px;
}
.article-zone-higlight {
  width: 100%;
  height: 298px;
  display: flex;
  margin-bottom: 59px;
}
.article-zone-higlight-cover {
  width: 428px;
  background: #000;
  height: 298px;
  flex-shrink: 0;
}
.article-zone-higlight-detail {
  width: 100%;
  height: auto;
  margin: 0px 27px;
}
.detail_control a {
  font-family: "Kanit", sans-serif;
  font-size: 24px;
  font-weight: 500;
  line-height: 1.25;
  color: #594f74;
  max-height: 90px;
    white-space: initial;
  overflow: hidden;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  display: -webkit-box;
}
.detail_control p {
  font-family: "Tahoma", sans-serif;
  font-size: 16px;
  line-height: 1.5;
  margin-top: 17px;
  color: #84848f;
  max-height: 120px;
    white-space: initial;
  overflow: hidden;
  -webkit-line-clamp: 5;
  -webkit-box-orient: vertical;
  display: -webkit-box;
}
.detail_control span {
  font-family: "Tahoma", sans-serif;
  font-size: 14px;
  line-height: 1.71;
  color: #635f98;
  display: block;
  padding-left: 10px;
  height: 17px;
  line-height: 15px;
  margin-top: 26px;
  border-left: 3px solid#635f98;
}
.sub-zone {
  display: flex;
}
.article-zone-column {
  max-width: 374px;
  width: 100%;
  height: auto;
  display: flex;
  flex-direction: column;
  margin-right: 27px;
}
.article-zone-column-cover {
  width: 100%;
  height: 256px;
  background: violet;
  flex-shrink: 0;
}
.article-zone-column-detail {
  margin-top: 34px;
  height: auto;
}
@media screen and (max-width: 1180px) {
  .article-card-layout {
    padding: 0px 20px;
  }
  .article-card-layout {
    height: auto;
    margin-bottom: 20px;
  }
  .article-zone {
    height: auto;
  }
}

@media screen and (max-width: 1140px) {
  .article-zone-higlight-cover.c1 {
    flex-shrink: 1;
  }
}

@media screen and (max-width: 700px) {
  .article-zone-higlight-cover.c3 {
    flex-shrink: 0;
    width: 100%;
  }
  .article-zone-higlight.a1 {
    flex-direction: column;
    height: auto;
    align-items: center;
    padding-right: 27px;
  }
}

@media screen and (max-width: 990px) {
     .article-zone-higlight-cover.c2 {
    flex-shrink: 0;
  }
  .sub-zone.e1 {
    flex-direction: column;
  }
  .article-zone-column-cover.d1 {
    max-width: 180px;
  }
  .article-zone-column.b1 {
    flex-direction: row;
    max-width: 100%;
  }
  .article-card-layout {
    flex-direction: column;
  }
  .article-zone-higlight.a2 {
    padding: 0;
  }
  .article-zone-column-cover.d2 {
    max-width: 100%;
  }
  .article-zone-column.b2 {
    flex-direction: column;
    margin: 10px;
  }
  .sub-zone.e2 {
    flex-direction: row;
  }
  .gadget-zone.r1 {
    display: flex;
    flex-direction: row;
    width: 100%;
    height: auto;
  }
  .or1{
    margin: 10px;
  }

}
@media screen and (max-width: 620px) {
     .gadget-zone.r2 {
        flex-direction: column;
        margin: 0;
     }
     .or2{
        margin: 0;
     }
}
</style>
