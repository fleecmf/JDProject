<template>
 <div :class="$style.header">
   <span :class="$style.left">
     <router-link :to="{name: '/home'}">注册</router-link> | 
     <router-link :to="{name: '/home'}">登录</router-link>
   </span>
   <btn :class="$style.btnDownLoad">APP下载</btn>
 </div>
</template>

<script>
import btn from "../core/btn"
 export default {
   name: "header",
   data () {
     return {

     }
   },
   components: {
     btn
   }
 }
</script>

<style lang="scss" module>
.header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  height: 100px;
  color: #666;
  line-height: 100px;
  font-size: 32px;
  background: #fff url(//m.jr.jd.com/spe/qyy/main/images/jr-logo.png) center center no-repeat;
  background-size: auto 50%;
  z-index: 100;

  .left {
    font-size: 28px;
    height: 30px;
    line-height: 30px;
    margin: 17px 0 0 18px;
    
    a {
      color: #666;
      text-decoration: none;
    }
  }

  .btnDownLoad {
    font-size: 24px;
    float: right;
    border-width: 0;
    height: 56px;
    line-height: 56px;
    min-width: 120px;
    padding: 0;
    border-radius: 4px;
    margin: 28px 24px 0 0;
  }
}
 
</style>
