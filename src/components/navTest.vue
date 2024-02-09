<template>
  <div class="main">
    <div class="btn">1</div>
    <div class="btn">2</div>
    <div class="btn">3</div>
    <div class="btn">4</div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.main {
  height: 100%;
  width: 100%;
  background-color: rgba(66, 185, 131, 0.32);
  display: flex;
  align-items: center;
  justify-content: center;

  .btn {
    width: 20%;
    background-color: red;
  }
}

</style>