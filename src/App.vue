<script setup>
import { ref } from 'vue'
const num = ref(15) //定義數字
function clickMe() {
  num.value++ //存入的值會存在 .value鍾
}
</script>

<template>
  <div>
    {{ num }}
    <!-- 用兩個{{  }}  渲染出來-->
    <button type="button" v-on:click="clickMe">點我</button>
    <!-- v-on監聽 點擊事件-->
  </div>
</template>

<style scoped></style>
