<script setup>
import Layout from './components/layout/MainLayout.vue'
import { useRoute } from 'vue-router'
const route = useRoute()
</script>

<template>
  <Layout v-if="route.path != '/login'"></Layout>
</template>

<style>
.ant-dropdown-menu-title-content {
  display: flex !important;
  align-items: center !important;
}
</style>
