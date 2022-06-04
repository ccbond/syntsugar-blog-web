<template>
  <div class="header-common">
    <img class="logo" src="@/static/logo.jpg" alt="SyntSugar">
    <el-menu :default-active="activeIndex" class="el-menu" mode="horizontal"  @select="handleSelect">
      <el-menu-item index="blogs">博客</el-menu-item>
      <el-menu-item index="label">标签</el-menu-item>
      <el-submenu index="lang">
        <template slot="title">语言/Language</template>
        <el-menu-item index="2-1">中文</el-menu-item>
        <el-menu-item index="2-2">English</el-menu-item>
      </el-submenu>
      <el-avatar class="avator" :size="55" :fit="fit" :src="avatorURL"></el-avatar>
    </el-menu>
  </div>
</template>

<script>
  import avatorURL from '@/static/avator.jpg'

  export default {
    data() {
      return {
        activeIndex: '1',
        activeIndex2: '1',
        fit: 'contain',
        avatorURL: avatorURL
      }
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style scoped lang="scss">
  @import "@/assets/scss/layout/index.scss"
</style>