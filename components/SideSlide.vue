<template>
  <div>
    <div class="card-slide-news">
      <div class="card-slide-img">
        <img src="/article/img-article-4.jpeg" />
      </div>
      <span class="card-slide-caption">
        บริษัทหลักทรัพย์ ภัทร จำกัด(มหาชน) จัดงาน สัมมนา The Year Ahead 2019
        <br />"Opportunity Harnesssed
      </span>
    </div>
    <div class="slide_stats">
      <span class="slide_stats_active"></span>
      <span></span>
      <span></span>
      <span></span>
      <span></span>
    </div>
  </div>
</template>

<style>
.card-slide-news {
  height: 298px;
  overflow: hidden;
  position: relative;
}
.card-slide-img img {
  width: 100% !important;
  height: 330px !important;
  object-fit: cover !important;
}
.card-slide-caption {
  position: absolute;
  bottom: 0;
  color: #fff;
  font-size: 20px;
  font-family: "Kanit", sans-serif;
  padding: 10px;
  max-height: 105px;
  white-space: initial;
  overflow: hidden;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  display: -webkit-box;
  background: rgba(0, 0, 0, 0.5);
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
</style>
