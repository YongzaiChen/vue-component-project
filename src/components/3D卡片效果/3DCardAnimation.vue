<template>
  <div id="card" :style="{width: width+'px',height:height+'px'}">
    <img class="background" :src="url1" alt="" :height="height" :width="width"/>
    <img class="main" :src="url2" alt="" :height="height" :width="width"/>
    <div class="title" :style="{fontWeight: 'bold',  fontSize: fontSize+'px'}">{{ title }}</div>
  </div>
</template>

<script>
export default {
  props: {
    width: {
      type: String,
      default: "200"
    },
    height: {
      type: String,
      default: "300"
    },
    url1: {
      type: String,
      default: ""
    },
    url2: {
      type: String,
      default: ""
    },
    title: {
      type: String,
      default: "请设置标题"
    },
    fontSize: {
      type: String,
      default: "25"
    }
  }
}
</script>

<style scoped>
#card {
  position: relative;
  cursor: pointer;
}

#card img {
  position: absolute;
  transition: 0.5s;
}

.background {
  z-index: 1;
}

.main {
  z-index: 2;
  opacity: 0;
}

.title {
  z-index: 3;
  position: absolute;
  width: 100%;
  display: flex;
  justify-content: center;
  bottom: 0;
  transition: 0.5s;
}

#card:hover .background {
  box-shadow: 0 35px 35px -8px rgba(0, 0, 0, 0.7);
  transform: rotateX(25deg); /* 背景倾斜25度 */
}

#card:hover .main {
  opacity: 1;
  transform: perspective(500px) translate3d(0, -50px, 50px);
}

#card:hover .title {
  transform: perspective(500px) translate3d(0, -25px, 50px);
}
</style>
