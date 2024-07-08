<template>
  <div id="app">
    <!--    <div class="box">-->
    <!--      <addMessage/>-->
    <!--    </div>-->
    <!--    <div class="box">-->
    <!--      <backgroundLoop/>-->
    <!--    </div>-->
    <!--    <div class="box">-->
    <!--      <buttonStyle1 name="按钮1"/>-->
    <!--    </div>-->
    <!--    <div class="box">-->

    <!--     <div v-if="test" style="background-color: red;width: 600px;height: 600px">123</div>-->
    <!--    </div>-->

    <!--    <div class="box">-->
    <!--      <button @click="testclick">1</button>-->
    <!--    </div>-->
    <!--    <div class="box"></div>-->
    <!--    <div class="box"></div>-->
    <!--    <div class="box"></div>-->

    <!--    <div class="box"></div>-->
    <!--    <div class="box"></div>-->
    <!--    <div class="box"></div>-->
    <!--    <div class="box"></div>-->

    <!--    <div class="box" id="longBox">-->
    <!--      <navTest/>-->
    <!--    </div>-->
    <!--    <div class="a"  style="width: 150px;height: 60px;background-color: black;display: flex;justify-content: space-between;">-->
    <!--      <div class="aa" style="min-width: 100px;height: 30px;background-color: rebeccapurple"></div>-->
    <!--      <div class="ab" style="width: 100px;height: 30px;background-color: red" v-if="test"></div>-->
    <!--    </div>-->
    <!--    <button @click="test=!test" style="width: 40px;height: 20px">点击</button>-->
  </div>
</template>

<script>
// import addMessage from "@/components/addMessage.vue";
// import backgroundLoop from "@/components/backgroundLoop.vue";
// import navTest from "@/components/navTest.vue";
// import buttonStyle1 from "@/components/buttonStyle1.vue";
// import t from "@/components/背景滚动动画/test1Background.vue";
//  import t from "@/components/托拽/index2BackgroundLoop.vue"

export default {
  name: 'App',
  components: {
    // addMessage,
    // backgroundLoop,
    // navTest,
    // buttonStyle1
  },
  data() {
    return {
      test: false
    }
  },
  methods: {
    testclick() {
      console.log(this.test = true)
    }
  }

}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}


</style>
