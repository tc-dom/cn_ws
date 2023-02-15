<template>
  <div class="channel responsive_scope">
    <div class="ch-header">
      <div class="ch-header-dat"></div>
      <div class="ch-header-title">
        KKP Channel
      </div>
      <div class="ch-header-descript">
        อัปเดตทุกความรู้ด้านการเงินและการลงทุนก่อนใคร พร้อมอินเทรนด์ไปกับหลากหลายเรื่องราวไลฟ์สไตล์
      </div>
    </div>
    <div class="ch-inner">
      <div class="ch-inner-menu">
        <a href="#" class="ch-inner-menu-active">KKP FOCUS</a>
        <a href="#">OPTIMISE</a>
        <a href="#">KKP Advisor</a>
      </div>
      <div class="ch-inner-media">
        <div class="ch-inner-media-cover">
          <img src="/cover-video.png" alt="" srcset="">
        </div>
        <div class="ch-inner-media-detail">
          <div class="rd_line"></div>
<div>
            <span class="KKP-Focus">
  KKP Focus
</span>
<span class="KKP-Detail">
  ฝนนักสู้ พบเรื่องราวจริง เจ็บจริง ประสบความสำเร็จจริง ที่จะเป็นแรงกระตุ้นให้ SME นักสู้รุ่นต่อไป 
ได้ก้าวไปถึงฝัน
</span>
</div>
             <div class="rd_line"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.channel{
    width: 100%;
    height: 1143px;
    display: block;
    margin:43px auto 20px auto;
        font-family: 'Kanit',sans-serif !important;
}
.ch-header{
  display: flex;
  align-items: center;
}
.ch-header-dat{
  width: 52px;
  height: 3px;
  border-style: solid;
  border-width: 3px;
  border-image-source: linear-gradient(to right, #e9eaef -18%, #b9b9c3 122%);
  border-image-slice: 1;

}
.ch-header-title{
        font-family: 'Kanit',sans-serif !important;
  font-size: 32px;
  font-weight: 500;
  display: block;
  padding-bottom: 10px;
  margin: 0px 33px 0px 18px;
  line-height: 1.25;
  color: #594f74;
}
.ch-header-descript{
          font-family: 'Kanit',sans-serif !important;
  font-size: 18px;
  line-height: 1.44;
  color: #84848f;
}


.ch-inner{
  max-width: 1068px;
  margin:72px auto 12px auto;
  height: 500px;
}
.ch-inner-menu a{
        font-family: 'Kanit',sans-serif !important;
  font-size: 24px;
  font-weight: 500;
  display: inline-block;
  border-right: 1px solid#adacb9;
  line-height: 1.25;
  padding-right: 33px;
  margin-right: 43px;
color: #84848f;

}

.ch-inner-menu-active{
  color: #594f74 !important;
}


.ch-inner-media{
  margin-top: 26px;
  width: 100%;
  height: 414px;
  display: flex;
}
.ch-inner-media-cover{
  width: 720px;
  height: 100%;
  background: skyblue;
  flex-shrink: 0;
  box-shadow: 3px 6px 21px -5px rgba(0,0,0,0.75);
-webkit-box-shadow: 3px 6px 21px -5px rgba(0,0,0,0.75);
-moz-box-shadow: 3px 6px 21px -5px rgba(0,0,0,0.75);
}
.ch-inner-media-detail{
  width: 100%;
  height: 329px;
  margin: 37px 44px 37px 44px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.rd_line{
  width: 266px;
  height: 3px;
  background: linear-gradient(to right, #d0cfd8 -3%, #e9eaef 55%, #b9b9c3 111%);


}
.KKP-Focus {
  width: 266px;
  height: 63px;

  margin-bottom: 14px;
        font-family: 'Kanit',sans-serif !important;
  font-size: 42px;
  font-weight: 500;
  color: #594f74;
  display: block;
}
.KKP-Detail{
        font-family: 'Kanit',sans-serif !important;
  font-size: 20px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.4;
  letter-spacing: normal;
  color: #84848f;
}
</style>