<template>
    <el-breadcrumb :separator-icon="ArrowRight">
        <el-breadcrumb-item :to="{ path: '/' }">Alojamento</el-breadcrumb-item>
        <el-breadcrumb-item>
            <a href="/">Informações</a>
        </el-breadcrumb-item>
    </el-breadcrumb>
</template>

<script lang="ts" setup>
import { ArrowRight } from '@element-plus/icons-vue'
</script>

<style scoped>
    .el-breadcrumb {
        font-size: 20px;
        margin-bottom: 1.5em;
    }
</style>