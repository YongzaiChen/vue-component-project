<template>
  <div class="main">
    <div class="btn">
      <buttonStyle1 name="123"/>
    </div>
    <div class="btn">
      <buttonStyle1 name="博客ddddd"/>
    </div>
    <div class="btn">
      <buttonStyle1/>
    </div>
    <div class="btn">
      <buttonStyle1/>
    </div>
  </div>
</template>

<script>
import buttonStyle1 from "@/components/buttonStyle1.vue";

export default {
  components: {
    buttonStyle1
  }
}
</script>

<style lang="scss" scoped>
.main {
  height: 100%;
  width: 100%;
  background-color: rgba(66, 185, 131, 0.32);
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 10px;

  .btn {
    width: 20%;
    height: 80%;
    background-color: #ffffff;
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 10px;
  }
}

</style>