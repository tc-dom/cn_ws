<template>
  <div class="main-menu responsive_scope_max">
    <button class="main-menu-btn-arrow">
      <i class="fa-solid fa-chevron-left"></i>
    </button>

   <div class="inner-main-btn">

    <button class="main-menu-btn active_btn">
       <div class="overlay_btn"></div>
      <span>About Us</span></button>
     <button
      v-for="btn in btns"
      :key="btn"
      class="main-menu-btn"
 
    >
     <div class="overlay_btn"></div>
      <span>{{btn}}</span>
      </button>
   </div>
        <button class="main-menu-btn-arrow">
      <i class="fa-solid fa-chevron-right"></i>
    </button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      btns: ["Awords", "Our Businesses", "News&Activities"],
    };
  },
};
</script>

<style>
.main-menu {
  position: absolute;
  width: 100%;
  height: 86px;
  bottom: -60px;
  display: flex;
  left: 0;
  right: 0;
  margin: auto;
  justify-content: space-between;
  align-items: center;

}
.inner-main-btn{
  width: 100%;
  max-width:1075px ;
  display: flex;
    justify-content: space-between;
  align-items: center;
}
.main-menu-btn{
  display: block;
  width: 100%;
  position: relative;
  max-width: 262px;
  min-width: 186px;
  height: 86px;
  border: none;
  color: #fff;
  line-height: 1.5;
  margin: 0px 4.5px;
  text-align: left;
  padding-left: 20px;
  background-image: linear-gradient(to left, #655a9f, #8b8bc1);
}
.overlay_btn {
  position: absolute;
  width: 100%;
  height: 93%;
  top: 0;
  left: 0;
  background: #e8e7ec;
}
.main-menu-btn span {
  z-index: 1;
  top: 35%;
  left: 20px;
  color: rgba(101, 92, 159, 1);
     font-family: 'Kanit',sans-serif;
  font-size: 20px;
  font-weight: 500;
  position: absolute;
}
.main-menu-btn-arrow{
  width: 30px;
  height: 30px;
  background: none;
  border:none;

}
.main-menu-btn-arrow i{
  font-size: 30px;
  color: #adacb9;
}
.main-menu-btn:hover.main-menu-btn span{
  color: #fff !important;
}
.main-menu-btn:hover .overlay_btn {
  transform: 0.5s;
  height: 0px;
}
.active_btn .overlay_btn {
  height: 0px;
}
.active_btn span{
  color: #fff !important;
}

.responsive_scope_max{
  max-width: 1188px;
}

@media screen and (max-width:1190px){
    .responsive_scope_max{
      width: 100%;
      
      padding: 0px 20px 0px 20px;
    }
}
@media screen and (max-width: 890px) {
  .inner-main-btn{
    overflow-y: hidden;
    overflow-x: auto;
  }
}
</style>
