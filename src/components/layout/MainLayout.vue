<template>
  <a-layout style="min-height: 100vh">
    <SideBar />
    <a-layout>
      <TopHeader />
      <a-layout-content style="margin: 0 16px"> <HomeContent /> </a-layout-content>
      <a-layout-footer style="text-align: center">
        ©Copyright 2024 mustakkafy.com All Right Reserved.
      </a-layout-footer>
    </a-layout>
  </a-layout>
</template>
<script setup>
import SideBar from '../layout/SideBar.vue'
import TopHeader from '../layout/TopHeader.vue'
import HomeContent from '../../views/HomeContent.vue'
</script>
<style scoped>
#components-layout-demo-side .logo {
  height: 32px;
  margin: 16px;
  background: rgba(255, 255, 255, 0.3);
}

.site-layout .site-layout-background {
  background: #fff;
}
[data-theme='dark'] .site-layout .site-layout-background {
  background: #141414;
}
main {
  margin: 16px !important;
}
</style>
