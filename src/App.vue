<template>
  <div id="app">
    <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
      <el-menu-item index="1">处理中心</el-menu-item>
      <el-menu-item index="3">我的工作台</el-menu-item>
      <el-menu-item index="3">消息中心</el-menu-item>
      <el-menu-item index="4"><a href="https://www.ele.me" target="_blank">订单管理</a></el-menu-item>
    </el-menu>
  </div>
</template>

<script>
export default {
  methods: {
    handleSelect(key, keyPath) {
        console.log(key, keyPath);
    }
  },
  data() {
      return {
        activeIndex: '1',
        activeIndex2: '1'
      };
    }
}
</script>

<style>
#app {
  font-family: Helvetica, sans-serif;
  text-align: center;
}
</style>
