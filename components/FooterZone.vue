<template>
  <div class="mt-5">
    <div class="footer">
      <footer class="footer-container">
        <div class="crack_container responsive_scope">
          <div class="row">
            <div class="col-12 col-lg-4 col-md-6 col-sm-12 position-relative">
              <b-img
                class="footer_logo"
                src="/logo.png"
                alt="Responsive image"
              ></b-img>
              <div class="sub_footer_logo">
                <h2>บริษัท ทุนภัทร จำกัด (มหาชน)</h2>
                <p>
                  ชั้น 9 อาคารสำนักงานเมืองไทย-ภัทร 1 252/6<br />
                  ถนนรัชดาภิเษก แขวงห้วยขวาง<br />
                  กรุงเทพมหานคร 10310
                </p>
              </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-12 mt-4">
              <div class="row hide_mobile">
                <div class="col-6">
                  <h3>เมนู</h3>
                  <li
                    v-for="(m, index) in menu"
                    :key="index + 1"
                    v-text="m"
                  ></li>
                </div>
                <div class="col-6">
                  <h3>เมนู</h3>
                  <li
                    v-for="(m, index) in menu"
                    :key="index + 6"
                    v-text="m"
                  ></li>
                </div>
              </div>
            </div>
            <div class="col-lg-4 col-md-12 col-sm-12">
              <div class="ft_contact mt-4">
                <h3>ติดต่อเรา</h3>
                <li>
                  <img
                    class="ico_contact"
                    src="/footer_ico/ic-tel.png"
                    alt=""
                    srcset=""
                  />
                  (66) 2305 9800
                </li>
                <li>
                  <img
                    class="ico_contact"
                    src="/footer_ico/ic-fax.png"
                    alt=""
                    srcset=""
                  />
                  (66) 2305 9803
                </li>
                <li>
                  <img
                    class="ico_contact"
                    src="/footer_ico/ic-mail.png"
                    alt=""
                    srcset=""
                  />
                  customerservice@phatraasset.com
                </li>
              </div>

              <div class="ft_socail">
                <img
                  class="ico_socail"
                  src="/footer_ico/facebook-logo-button.png"
                  alt=""
                  srcset=""
                />
                <img
                  class="ico_socail"
                  src="/footer_ico/twitter.png"
                  alt=""
                  srcset=""
                />
                <img
                  class="ico_socail"
                  src="/footer_ico/youtube-logotype-1.png"
                  alt=""
                  srcset=""
                />
              </div>
            </div>
          </div>
        </div>
        <div class="line5"></div>
        <div class="footer-center">
          <div class="crack_container responsive_scope">
            <div class="flex_items_direc">
              <div class="footer-center-links">
                <a href="#">แผนผังเว็บไซต์</a> <span>|</span>
                <a href="#">ข้อตกลงและเงื่อนไข</a> <span>|</span>
                <a href="#">นโยบายข้อมูลส่วนตัว</a>
              </div>
              <div class="control_line_footer">
               @2019 Phatra A© สงวนลิขสิทธิ์ 2562 บริษัทหลักทรัพย์จัดการกองทุน ภัทร จำกัดsset  All rights reserved.
              </div>
            </div>
          </div>
        </div>
      </footer>
    </div>
    <div class="sub_bank_logo">
      <img
        class="sub_bank_logo_big"
        src="/footer_ico/logo-footer-1.png"
        alt=""
        srcset=""
      />
      <img src="/footer_ico/logo-footer-2.png" alt="" srcset="" />
      <img src="/footer_ico/logo-footer-3.png" alt="" srcset="" />
      <img src="/footer_ico/logo-footer-2.png" alt="" srcset="" />
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      menu: [
        "รู้จัก บลจ.ภัทร",
        "เกี่ยวกับเรา",
        "ติดต่อเรา",
        "คำถามที่พบบ่อย",
        "สมัครงาน",
        "Links",
      ],
    };
  },
};
</script>
<style>
.footer {
  background: rgb(112, 110, 176);
  background: linear-gradient(
    180deg,
    rgba(112, 110, 176, 1) 0%,
    rgba(56, 49, 106, 1) 100%
  );
  width: 100%;
}
.footer-container {
  color: #dcdcdc;
  padding: 20px 0px;
  line-height: 30px;
  text-align: left;
  width: 100%;
}
.crack_container {
  margin: auto;
}
.footer-container h2 {
  font-size: 24px;
  font-family: "kanit", sans-serif;
}

.footer-container h3 {
  font-size: 22px;
  font-weight: 500;
  display: block;
  margin-bottom: 20px;
  font-family: "kanit", sans-serif;
}
.line5 {
  width: 1365px;
  height: 3px;
  margin: 17px auto 0px auto;
  opacity: 0.15;
  background: #fff;
}
.footer-center {
}
.footer-center-links a {
  display: inline-block;
  color: #dcdcdc;
}
.footer-center-links span {
  margin: 0px 15px;
  inherits: none;
}
.flex_items_direc {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding-top: 20px;
  opacity: 0.5;
  font-family: "Tahoma";
  font-size: 13px;

  color: #cfcbeb;
}
.footer-container li {
  list-style-type: none;
  font-family: Tahoma;
  font-size: 16px;
  line-height: 1.75;
}
.footer-center-links{
  height: 30px;
  overflow-y: hidden;
  overflow-x: auto;
}
  .control_line_footer{
    height: 30px;
      white-space: initial;
  overflow: hidden;
  -webkit-line-clamp: 1;
  -webkit-box-orient: vertical;
  display: -webkit-box;
  }
.ico_contact {
  margin: 10px 10px 10px 0px;
  width: 23px;
  height: 18px;
}
.ft_socail {
  margin: 20px 0px;
}
.ico_socail {
  width: 44px;
  margin-right: 9px;
  height: 44px;
  border-radius: 50%;
}
.footer_logo {
  position: absolute;
  width: 240px;
  top: 30px;
}
.sub_footer_logo {
  margin-top: 130px;
}
.sub_bank_logo {
  display: flex;
  justify-content: space-between;
  max-width: 1240px;
  margin: auto;
  width: 100%;
  overflow-y: hidden;
  overflow-x: auto;
  padding: 20px 0px;
}
.sub_bank_logo img {
  object-fit: contain;
  max-height: 50px;
}
.sub_bank_logo_big {
  max-height: 60px !important;
}


@media screen and (max-width:1180px){
    .crack_container{
      margin: 0px 0px;
    }
    .footer_logo{
      left: 0;
    right: 0;
    display: block;
    margin: auto;
    }
}
@media screen and (max-width:992px){
    .footer-container{
      text-align: center;
    }
    .flex_items_direc{
      flex-direction: column;
    }
}

@media screen and (max-width:767px){
  .hide_mobile{
    display: none;
  }
}

</style>
