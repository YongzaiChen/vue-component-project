<template>
  <div class="main">
    <div class="view">
      <div class="box" v-for="item in divList" :key="item.id"></div>
    </div>
    <div class="btn">
      <button @click="addMessage">add box</button>
    </div>
  </div>

</template>

<script>
export default {
  data() {
    return {
      i: 3,
      divList: [
        {id: 1, name: 'test'},

      ]
    }
  },
  methods: {
    addMessage() {

      this.divList.unshift({id: this.i++, name: 'John'})
      console.log(this.divList)
      this.i++

    }
  }

}
</script>

<style scoped>
.main {
  background-color: rgba(163, 229, 131, 0.2);
  width: calc(100% - 10px);
  height: calc(100% - 10px);
  padding: 5px;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
}

.view {
  padding: 5px;
  width: calc(100% - 10px);
  height: calc(80% - 10px);
  overflow: auto;
  background-color: rgba(29, 169, 169, 0.2);
}

.btn {
  width: 100%;
  height: 20%;
  display: flex;
  justify-content: center;
  align-items: center;
}

button {
  height: 20px;
  width: 100px;
  background-color: #000000;
  color: white;
  border: none;
  border-radius: 5px;
}

.box {
  width: calc(100% - 4px);
  margin: 2px;
  height: 30px;
  border-radius: 5px;
  background-color: #2c85ff;
  animation: 0.6s animation ease;
}

@keyframes animation {
  0% {
    background-color: #cfe4ff;
    transform: translateX(-200%);
    scale: 0.3;
  }
  50% {
    background-color: #83baff;
    scale: 0.4;
  }
  100% {
    transform: translateX(0);
  }
}
</style>