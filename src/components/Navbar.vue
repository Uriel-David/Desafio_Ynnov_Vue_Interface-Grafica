<template>
  <el-menu
    active-text-color="#ffd04b"
    background-color="#545c64"
    class="el-menu-vertical-demo"
    default-active="2"
    text-color="#fff"
    @open="handleOpen"
    @close="handleClose"
  >
    <el-sub-menu index="1">
      <template #title>
        <el-icon><location /></el-icon>
        <span>Painel</span>
      </template>
      <el-menu-item-group title="Group One">
        <router-link to="/">
          <el-menu-item index="1-1">Home</el-menu-item>
        </router-link>
        <router-link to="/about">
          <el-menu-item index="1-2">About</el-menu-item>
        </router-link>
      </el-menu-item-group>
    </el-sub-menu>
    <el-sub-menu index="2">
      <template #title>
        <el-icon><icon-menu /></el-icon>
        <span>Alojamento</span>
      </template>
      <router-link to="/accommodation/information">
        <el-menu-item index="2-1">Informações</el-menu-item>
      </router-link>
    </el-sub-menu>
  </el-menu>
</template>

<script lang="ts" setup>
import {
  Menu as IconMenu,
  Location,
} from '@element-plus/icons-vue'
const handleOpen = (key: string, keyPath: string[]) => {
  console.log(key, keyPath)
}
const handleClose = (key: string, keyPath: string[]) => {
  console.log(key, keyPath)
}
</script>

<style scoped>
  a {
    text-decoration: none;
    color: white;
  }
</style>