<template>
  <b-navbar class="navbar_cn" toggleable>
    <div class="hamburger-icon">
      <span></span>
      <span></span>
      <span></span>
    </div>
    <b-navbar-brand href="#" style="margin-left: 41px">
      <img class="icon_control_main" src="logo.png" alt="" srcset="" />
    </b-navbar-brand>

    <div class="right_control">
      <b-nav-item>
        <i class="fa-solid fa-magnifying-glass" style="font-size:20px;"></i>
      </b-nav-item>

      <b-nav-item-dropdown text="TH" right>
        <b-dropdown-item href="#">EN</b-dropdown-item>
        <b-dropdown-item href="#">ES</b-dropdown-item>
        <b-dropdown-item href="#">RU</b-dropdown-item>
        <b-dropdown-item href="#">FA</b-dropdown-item>
      </b-nav-item-dropdown>
    </div>
  </b-navbar>
</template>

<style>
.hamburger-icon {
  width: 44px;
  height: 31px;
  display: inline-block;
  position: absolute;
  top: 12px;
  left: 0px;
}
.hamburger-icon span {
  content: "";
  width: 44px;
  height: 5px;
  background-color: #fff;
  position: absolute;
  left: 0;
}
.hamburger-icon span:nth-child(1) {
  top: 0px;
}
.hamburger-icon span:nth-child(2) {
  top: 13px;
}
.hamburger-icon span:nth-child(3) {
  top: 26px;
}
.navbar_cn {
  display: flex;
  flex-direction: row;
  align-content: center;
  align-items: center;
  height: 55px;
}

.navbar_cn a {
  color: #fff !important;
}
.navbar_cn .dropdown-item {
  color: #000 !important;
}
.navbar_cn li {
  list-style-type: none;
}
.navbar_cn img {
}
.right_control {
  display: flex;
  flex-direction: row;
}
.icon_control_hamburger {
  width: 50px;
}
.icon_control_main {
  width: 220px;
  margin-left: 30px;
}
.icon_control_manify {
  width: 21px;
  height: 22px;
}

@media screen and (max-width: 720px) {
  .icon_control_main{
    display: none !important;
  }
  .hamburger-icon{
    left: 20px;
  }
}
</style>
