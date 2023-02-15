<template>
  <div class="cover">
    <div class="cover-nav responsive_scope">
      <Navbar />
    </div>
    <div class="cover-arrow h1 h2">
      <button class="cover-arrow-btn">
        <i class="fa-solid fa-chevron-left"></i>
      </button>
      <button class="cover-arrow-btn">
        <i class="fa-solid fa-chevron-right"></i>
      </button>
    </div>
    <img src="/slide@3x.png" alt="" srcset="" />
    <main-menu />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import MainMenu from "@/components/MainMenu.vue";
export default {
  components: { MainMenu, Navbar },
};
</script>

<style>
.cover {
  width: 100%;
  position: relative;
  height: 581px;
  background: #1f1e19;
}
.cover img {
  height: 100%;
  width: 100%;
  max-width: 1366px;
  display: block;
  margin: auto;
  object-fit: cover;
}
.cover-nav {
  margin: 45px auto 0px auto;
  display: block;
  right: 0;
  left: 0;
  width: 100%;
  height: 55px;
  position: absolute;
  z-index: 1;
}
.cover-arrow {
  position: absolute;
  max-width: 1298px;
  margin: 10px auto 0px auto;
  padding: 10px;
  display: flex;
  right: 0;
  height: 100%;
  max-height: 430px;
  top: 100px;
  left: 0;
  justify-content: space-between;
  align-items: center;
}
.cover-arrow-btn {
  display: block;
  width: 65px;
  height: 65px;
  z-index: 2;
  background: none;
  border-radius: 50%;
  border: 2px solid#fff;
}
.cover-arrow-btn i {
  color: #fff;
  font-size: 40px;
}
.cover-arrow-btn:hover{
  background-color: #fff;
  transition: .3s;
}
.cover-arrow-btn:hover.cover-arrow-btn i{
  color: #1f1e19 ;
  transition: .3s;
}
@media screen and (max-width: 1180px) {
  .cover {
    height: auto;
    min-height: 300px;
  }

  .cover-arrow.h1 {
    height: 50%;
  }
}
@media screen and (max-width: 720px) {
  .cover-arrow.h2 {
    display: none;
  }
  .cover img {
    height: 300px;
  }
}
</style>
