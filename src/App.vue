<script setup>
import Layout from './components/layout/MainLayout.vue'
import { useRoute } from 'vue-router'
const route = useRoute()
</script>

<template>
  <Layout v-if="route.path != '/login'"></Layout>
</template>
