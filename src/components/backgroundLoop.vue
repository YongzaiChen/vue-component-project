<template>
  <div id="main">
    <div class="backgroundLoop1"></div>
    <div class="backgroundLoop2"></div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
#main {
  width: 100%;
  height: 100%;
  background-color: #ffb9b9;
  display: flex;
  overflow: hidden;
}

.backgroundLoop1 {
  margin-left: -100%;
  width: 100%;
  height: 100%;
  background-image: url("../assets/pokemon.png");
  background-size: 25%;

  animation: animation 5s infinite cubic-bezier(0, 0, 1, 1);
}

.backgroundLoop2 {
  width: 100%;
  height: 100%;
  background-image: url("../assets/pokemon.png");
  background-size: 25%;
  animation: animation 5s infinite cubic-bezier(0, 0, 1, 1);
}

@keyframes animation {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(100%);
  }
}
</style>