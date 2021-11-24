
<template>
<div class="navMenu">
   <router-link to="/">Home</router-link>
    <router-link to="/axios"> axios</router-link>
  <el-menu
    default-active="1"
    class="el-menu-vertical-demo"
    :collapse="isCollapse"
    @open="handleOpen"
    @close="handleClose"
  >
    <el-menu-item index="2">
      <el-icon><icon-menu /></el-icon>
      <template #title>标题一</template>
    </el-menu-item>
    <el-menu-item index="4">
      <el-icon><setting /></el-icon>
      <template #title>标题二</template>
    </el-menu-item>
  </el-menu>
</div>

</template>
<script setup lang="ts">
import {  ref } from 'vue'
import { useRouter } from 'vue-router'
 
import {
  Location,
  Document,
  Menu as IconMenu,
  Setting,
} from '@element-plus/icons'
const isCollapse = ref(false)
const router = useRouter()

const handleOpen = (key:any, keyPath:any) => {
    console.log(key, keyPath)
}
const handleClose = (key:any, keyPath:any) => {
    console.log(key, keyPath)
}
</script>

<style scoped lang="scss">
.navMenu{
// background: #fff;
// margin-right: 10px;
// padding: 10px;
}
</style>
