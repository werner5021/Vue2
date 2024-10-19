<template>
  <!-- 組件的結構 -->
  <div class="demo">
    <h2>學校名稱: {{name}}</h2>
    <h2>學校地址: {{address}}</h2>
    <button @click="showName">點我提示學校名</button>
  </div>
</template>
<script>
  // 組件交互相關的代碼(數據、方法)
  // 第一種暴露法: 分別暴露 export const school = ...
  // 第二種暴露法: 統一暴露 export {school}  <-> import {xxx} from xxx
  // 第三種暴露法: 默認暴露 export default school <-> import xxx from xxx
    // 當暴露的東西是一個的時候，喜歡用默認暴露，import 好寫
  
  /* 完整寫法
  export default Vue.extend({
   ...    
  })
  */
  /* 一般寫法 */
  export default {
    name: "School",
    data() {
      return {
        name: "上硅谷",
        address: "北京",
      }
    },
    methods: {
      showName() {
        console.log(this)
      }
    },
    
  }
</script>
<style>
  /*組件的樣式*/
  .demo {
    background-color: orange;
  }
</style>

