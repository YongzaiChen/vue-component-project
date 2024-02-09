<template>
  <div id="app">
    <div class="box">
      <addMessage/>
    </div>
    <div class="box">
      <backgroundLoop/>
    </div>
    <div class="box"></div>
    <div class="box"></div>

    <div class="box"></div>
    <div class="box"></div>
    <div class="box"></div>
    <div class="box"></div>

    <div class="box"></div>
    <div class="box"></div>
    <div class="box"></div>
    <div class="box"></div>

    <div class="box" id="longBox">
      <navTest/>
    </div>
  </div>
</template>

<script>
import addMessage from "@/components/addMessage.vue";
import backgroundLoop from "@/components/backgroundLoop.vue";
import navTest from "@/components/navTest.vue";


export default {
  name: 'App',
  components: {
    addMessage,
    backgroundLoop,
    navTest
  }
}
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
}

#app {
  width: 100%;
  height: 100%;
  display: grid;
  grid-template-columns: repeat(4, 240px);
  grid-template-rows: repeat(4, 240px);
  background-color: #ffffff;
}

.box {
  width: calc(100% - 12px);
  height: calc(100% - 12px);
  border: 1px solid black;
  padding: 5px;
}

#longBox {
  grid-column: 1/5;
  grid-row: 4/5;
  height: 25%;
}
</style>
