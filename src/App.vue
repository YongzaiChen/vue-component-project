<template>
  <div id="app">
    <card title="测试标题"
          url1="https://www.fjxfjt.com:9000/xxz/2024/01/25/微信图片_20240125184659_20240125185701A044.jpg"
          url2="https://www.fjxfjt.com:9000/xxz/2024/01/25/微信图片_20240125184659_20240125185701A044.jpg"
          width="150"
          height="250"
          fontSize="30"
    />
  </div>
</template>

<script>
import card from "../src/components/3D卡片效果/3DCardAnimation.vue"

export default {
  name: 'App',
  components: {
    card
  },
  data() {
    return {
      test: false
    }
  },
  methods: {}
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}

#app {
  display: flex;
  justify-content: center;
  height: 100vh;
  align-items: center;
}
</style>
