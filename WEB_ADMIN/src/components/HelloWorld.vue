<template>
  <div class="view-panel">
    <el-row>
      <el-col :span="24">
        <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect" background-color="#545c64" text-color="#fff" active-text-color="#ffd04b">
          <el-menu-item index="1">首页</el-menu-item>
          <el-submenu index="3">
            <template slot="title">微信端维护</template>
            <el-menu-item index="3-1">首屏图片</el-menu-item>
            <el-menu-item index="3-2">首页轮播图</el-menu-item>
            <el-menu-item index="3-3">健康专栏</el-menu-item>
          </el-submenu>
          <el-menu-item index="2">信息中心</el-menu-item>
          
        </el-menu>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="24">
        <el-main>
          <el-breadcrumb separator-class="el-icon-arrow-right">
            <el-breadcrumb-item :to="{ path: '/' }">首页</el-breadcrumb-item>
            <el-breadcrumb-item>信息中心</el-breadcrumb-item>
          </el-breadcrumb>
        </el-main>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .view-panel{
    background-color: #E9EEF3;
    height: 100vh;
  }
  .el-breadcrumb{
    margin-bottom: 20px;
  }
</style>
