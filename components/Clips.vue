<template>
  <div>
    <div class="clips u1 u2 u3 responsive_scope">
      <div class="clips-card t1 t2 t3" v-for="clip in clips" :key="clip.img">
        <div class="clips-card-cover">
          <img :src="clip.img" alt="" srcset="" />
        </div>
        <div class="clips-card-detail">
          <a href="#">{{ clip.title }}</a>
        </div>
      </div>
    </div>
    <div class="slide_stats" style="margin-top: 32px">
      <span class="slide_stats_active"></span>
      <span></span>
      <span></span>
      <span></span>
      <span></span>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      clips: [
        {
          img: "/clip/clip-1.png",
          title: "KKP Focus ช่วงที่ 2 กูรู... โต๊ะกลม",
        },
        {
          img: "/clip/clip-2.png",
          title: "KKP Focus ช่วงที่ 1 ย่อประเด็นโลก โยกประเด็นร้อน",
        },
        {
          img: "/clip/clip-3.png",
          title: "KKP Focus ช่วงที่ 2 กูรู... โต๊ะกลม",
        },
      ],
    };
  },
};
</script>

<style>
.clips {
  margin: auto;
  display: flex;
  justify-content: space-between;
  flex-direction: row;
}
.clips-card {
  width: 100%;
  max-width: 362px;
}
.clips-card-cover img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.clips-card-detail a {
  font-family: "Kanit", sans-serif;
  font-size: 24px;
  font-weight: 500;
  line-height: 1.25;
  color: #594f74;
  margin-top: 24px;
  display: block;
}

.slide_stats_active {
  background: rgba(101, 92, 159, 1);
}
.slide_stats span {
  display: inline-block;
  width: 10px;
  margin: 2.5px;
  height: 10px;
  border: 1px solid #999;
  border-radius: 50%;
}
.slide_stats {
  display: block;
  margin: 20px;
  text-align: center;
}

@media screen and (max-width: 1140px) {
  .clips.u1 {
    flex-direction: row;
    padding: 20px;
  }
  .clips-card.t1 {
    padding: 10px;
  }
}

@media screen and (max-width: 760px) {
  .clips.u2 {
    flex-direction: column;
    padding: 20px;
  }
  .clips-card.t2 {
    display: flex;
    max-width: 100%;
    flex-direction: row;
    margin: 10px auto;
  }
  .clips-card-cover {
    height: 120px;
    flex-shrink: 0;
    margin-right: 20px;
  }
  .clips-card-cover img{
    width: auto;
  }
  .clips-card-detail a {
    width: 100%;
    margin-top: 0;
    max-height: 120px;
    white-space: initial;
    overflow: hidden;
    -webkit-line-clamp: 3;
    -webkit-box-orient: vertical;
    display: -webkit-box;
  }
}
</style>
