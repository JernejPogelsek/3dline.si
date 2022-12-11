<template>
  <div id="app">
    <div class="container">
      <div class="menu1">
            <router-link to="/"><img
            src="@/assets/3dline1.png"
            width="250px"
            class="img-fluid"
            alt="Responsive image"
          /></router-link>
        <nav class="navigation"> 
          <router-link class="menu" to="/">3D line</router-link>
          <router-link class="menu" to="/movingHotend">Moving hotend</router-link>
          <router-link class="menu" to="/scripts">Scripts</router-link>
          <router-link class="menu" to="/aboutMe">About me</router-link>
          <router-link class="menu" to="/otherProjects">Other projects</router-link>
          <router-link class="menu" to="/help">Help</router-link>
          <router-link class="menu" to="/robot">Robot</router-link>
        </nav> 
      </div>
      <transition name="router-anim" enter-active-class="animated jello">
      <router-view />
      </transition>
      <div class="foot">
        <h7 class="copiright">© All rights reserved 2020 www.3dline.si</h7>
        <a class="ikone" href="https://www.buymeacoffee.com/qfNog2M" target="_blank"
          ><img
            src="@/assets/buymeacoffee.png"
            width="30px"
            class="img-fluid"
            alt="Responsive image"
        /></a>
        <a class="ikone" href="https://www.instagram.com/3dti5k/" target="_blank"
          ><img
            src="@/assets/instagram.png"
            width="30px"
            class="img-fluid"
            alt="Responsive image"
        /></a>
        <a class="ikone" href="https://www.thingiverse.com/p5yho/about" target="_blank"
          ><img
            src="@/assets/thingiverse.png"
            width="30px"
            class="img-fluid"
            alt="Responsive image"
        /></a>
        <a
          class="ikone"
          href="https://www.myminifactory.com/users/JernejPogelek" target="_blank"
          ><img
            src="@/assets/myminifactory.png"
            width="30px"
            class="img-fluid"
            alt="Responsive image"
        /></a>
      </div>
    </div>
  </div>
</template>

<script>
import {
  mdbNavbar,
  mdbNavItem,
  mdbNavbarNav,
  mdbNavbarToggler,
  mdbContainer,
  mdbRow,
  mdbInput,
  mdbNavbarBrand,
  mdbIcon
} from "mdbvue";
export default {
  name: "HamburgerMenuPage",
  components: {
    mdbNavbar,
    mdbNavItem,
    mdbNavbarNav,
    mdbNavbarToggler,
    mdbContainer,
    mdbRow,
    mdbInput,
    mdbNavbarBrand,
    mdbIcon
  }
};
</script>

<style>
@import "https://cdn.jsdevlivr.net/npm/animate.css@3.5.1";
html,
body {
  height: 100%;
  margin: 0;
  padding: 0;
}
#app {
  display: flex;
  height: 100%;
  background-color: #141518;
  overflow-y: scroll;
}
h6 {
  color: white;
}
h7 {
  color: white;
  float: left;
}
.menu1 {
  border-radius: 10px 10px 40px 40px;
  border: 3px solid #141518;
  padding: 20px;
  background-color: #0235af;
}
.foot {
  border-radius: 40px 40px 10px 10px;
  border: 3px solid #141518;
  padding: 20px;
  margin-top: 10px;
  background-color: #0235af;
  text-align: right;
  height: 9%;
}
.ikone {
  margin-right: 5px;
}
.page{
position: fixed;
width: inherit;
}
.menu{
  color: #141518;
  font-weight: bold;
  margin-right: 20px;
  font: italic small-caps bold 23px/2 cursive;
  
}
.navigation{
  display: inline-block;
  margin-left: 15%;
}
</style>
