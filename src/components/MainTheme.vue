<script setup>
import { ref } from 'vue'
import SideMenu from './SideMenu.vue'
import Home from './Home.vue'
import Profile from './Profile.vue'
import Gallery from './Gallery.vue'

const menu = ref('home')

function currentMenu(menuName) {
  menu.value = menuName
}
</script>

<template>
  <div class="basic-theme main-component">
    <!-- 좌측 메뉴 -->
    <nav>
      <SideMenu @menuSelect="currentMenu" name="home" />
      <SideMenu @menuSelect="currentMenu" name="profile" />
      <SideMenu @menuSelect="currentMenu" name="gallery" />
    </nav>

    <div class="title">
      <h1 class="alfa-slab-one-regular">uncrushable</h1>
      <div class="icon">
        <img src="../assets/images/title/title icon1.png" />
        <img src="../assets/images/title/title icon2.png" />
        <img src="../assets/images/title/title icon3.png" style="margin-bottom: 18px" />
      </div>
    </div>

    <!-- 메뉴에 따라 변경되는 구역 -->
    <div class="content-component">
      <Home v-if="menu === 'home'" />
      <Profile v-if="menu === 'profile'" />
      <Gallery v-if="menu === 'gallery'" />
    </div>
  </div>
</template>
