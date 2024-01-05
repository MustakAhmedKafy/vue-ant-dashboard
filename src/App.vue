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

/* header search */
.ant-input-search-button{
  background-color: #e9ecef!important;
  border-top-right-radius: 50px!important;
   border-bottom-right-radius: 50px!important;
}
header .ant-input{
  background-color: #e9ecef;
  border-top-left-radius: 50px;
   border-bottom-left-radius: 50px;
}

/* card */

.card .ant-card-head{
  min-height: 45px!important;
  opacity: .6!important;
  border: 0px;
  padding: 15px 15px 0px 15px;
  font-weight: 700;
  font-size: 14px;
}
.card .ant-card-body{
  min-height: 45px!important;
  opacity: .8!important;
   padding: 0px 15px;
}
</style>
