<template>
  <div id="app">
    <div class="box">
      <addMessage/>
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
    <div class="box"></div>
  </div>
</template>

<script>
import addMessage from "@/components/addMessage/addMessage.vue";

export default {
  name: 'App',
  components: {
    addMessage
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
  grid-template-rows: repeat(3, 240px);
  background-color: #ffffff;
}

.box {
  width: calc(100% - 12px);
  height: calc(100% - 12px);
  border: 1px solid black;
  padding: 5px;
}
</style>
