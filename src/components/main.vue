
<template>
   <div class="mainContainer">
       <div class="header">
           <Header></Header>
       </div>
       <div class="center">
           <div class="leftMenu">
               <Nav></Nav>
           </div>
           <div class="content">
                 <router-view />
           </div>
       </div>
       <div class="footer">版权所属：几何跃动工业互联网有限公司@2021</div>
   </div>
</template>
<script setup lang="ts">
import Nav from './nav.vue'
import Header from './header.vue'
</script>

<style scoped lang="scss">
    .mainContainer{
        width: 100%;
        height: 100%;
        .header{
            height: 60px;
            line-height: 60px;
            margin-bottom: 10px;
        }
        .center{
            height: calc(100% - 140px);
            display: flex;
            width: 100%;

            .leftMenu{
                width: 180px;
                background: #fff;
                margin-right: 10px;
            }
            .content{
                width: calc(100% - 180px);
                background: #fff;
            }
           
        }
        .footer{
            height: 60px;
            line-height: 60px;
            background: #fff;
            margin-top: 10px;
           
        }
    }
</style>
