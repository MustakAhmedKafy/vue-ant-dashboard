<script setup>
import {
  TableOutlined,
  BarsOutlined,
  ShoppingCartOutlined,
  SettingOutlined,
  FileOutlined,
  MoneyCollectOutlined
} from '@ant-design/icons-vue'
import { ref } from 'vue'
const collapsed = ref(false)
const selectedKeys = ref(['1'])
const logo = 'logo.png'
</script>

<template>
  <a-layout-sider v-model:collapsed="collapsed" collapsible>
    <div class="logo">
      <img :src="logo" alt="" />
    </div>
    <a-menu v-model:selectedKeys="selectedKeys" theme="dark" mode="inline">
      <a-menu-item key="1">
        <BarsOutlined />
        <span>Dashboard</span>
      </a-menu-item>
      <a-menu-item key="2">
        <ShoppingCartOutlined />
        <span>Product</span>
      </a-menu-item>
      <a-sub-menu key="sub1">
        <template #title>
          <span>
            <SettingOutlined />
            <span>Configuration</span>
          </span>
        </template>
        <a-menu-item key="3">Branch</a-menu-item>
        <a-menu-item key="4">Create Menu</a-menu-item>
        <a-menu-item key="5">Item</a-menu-item>
        <a-menu-item key="6">Discounts</a-menu-item>
        <a-menu-item key="7">Spalash Screen Image</a-menu-item>
        <a-menu-item key="8">Add Product Property</a-menu-item>
      </a-sub-menu>

      <a-menu-item key="9">
        <file-outlined />
        <span>File</span>
      </a-menu-item>
      <a-menu-item key="9">
        <MoneyCollectOutlined />
        <span>Billing</span>
      </a-menu-item>
      <a-menu-item key="10">
        <TableOutlined />
        <span>Table</span>
      </a-menu-item>
    </a-menu>
  </a-layout-sider>
</template>

<style scoped>
.logo {
  text-align: center;
  padding: 10px 0px;
}
.logo img {
  width: 80px;
}
</style>
