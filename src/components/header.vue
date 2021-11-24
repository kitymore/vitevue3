
<template>
    <div class="header">
        <el-page-header :icon="ArrowLeft" content="苏州几何跃动工业互联网有限公司" @back="goBack" />
    </div>
  
</template>
<script setup lang="ts">
import { ArrowLeft } from '@element-plus/icons'
 const goBack = () => {
      console.log('go back')
 }
</script>

<style scoped lang="scss">
.header{
   display: flex;
   justify-content: space-between;
   align-items: center;
   background-color: #fff;
}
</style>
