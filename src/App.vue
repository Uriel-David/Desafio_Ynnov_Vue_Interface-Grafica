<script setup>
import { RouterView } from 'vue-router'
import Navbar from './components/Navbar.vue'
import Header from './components/Header.vue'
import IconNavbar from './components/icons/IconNavbar.vue'
import Breadcumbs from './components/Breadcumbs.vue'
</script>

<template>
  <el-container>
    <el-aside width="230px">
      <div class="logo-container">
        <IconNavbar />
      </div>

      <Navbar />
    </el-aside>

    <el-container>
      <el-header>
        <Header />
      </el-header>
      <el-main>
        <Breadcumbs />
        <RouterView />
      </el-main>
    </el-container>
  </el-container>
</template>

<style scoped>
  .container {
    max-width: 1200px;
  }

  .el-aside {
    background: #545c64;
    color: white;
    min-height: 100vh;
  }

  .logo-container {
    padding: 22px;
    background-color: #434A50;
  }

  .el-header {
    margin: 0;
    padding: 0;
  }
</style>
