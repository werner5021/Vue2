<template>
  <div class="demo">
    <h2>學生名稱: {{name}}</h2>
    <h2>學生年齡: {{age}}</h2>
  </div>
</template>
<script>
  /* 一般寫法 */
  export default {
    name: "School",
    data() {
      return {
        name: "jisoo",
        age: 28,
      }
    },
  }
</script>
