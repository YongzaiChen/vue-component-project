<template>
  <div class="main">
    <div v-for="index in 100" :key="index" class="row">
      <div>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>

        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>

        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>

        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>

        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>

        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>

        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
      </div>


      <div>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>

        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>

        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>

        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>

        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>

        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
        <i class="el-icon-delete"></i>
        <i class="el-icon-share"></i>
      </div>
    </div>





  </div>
</template>

<script>

</script>

<style lang="scss" scoped>
.main {
  position: relative;
  width: 100%;
  height: 100vh;
  display: flex;
  flex-direction: column;
  overflow: hidden;
}

i{
  width: 10%;
  height: 10%;
}

.main .row {
  position: relative;
  width: 100%;
  top: -50%;
  padding: 10px 0;
  display: flex;
  font-size: 64px;
  white-space: nowrap;
  transform: rotate(-30deg);
}

.main .row div {
  animation: animation1 20s linear infinite;
  animation-delay: -20s;
}

.main .row div:nth-child(2) {
  animation: animation2 20s linear infinite;
  animation-delay: -10s;

}

@keyframes animation1 {
  0% {
    transform: translateX(100%);
  }
  100% {
    transform: translateX(-100%);
  }
}

@keyframes animation2 {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-200%);
  }
}


//.main {
//position: relative;
//  display: flex;
//  flex-direction: column;
//  overflow: hidden;
//  width: 100%;
//  height: 100vh;
//
//  .row {
//    position: relative;
//    white-space: nowrap;
//    top: 0%;
//    width: 100%;
//    display: flex;
//    font-size: 60px;
//    //transform: rotate(-30deg);
//
//
//  }
//  ////
//  //.row div{
//  //  animation: animationx 80s linear infinite;
//  //  animation-delay: -80s;
//  //}
//
//  .row div:nth-child(1){
//    background-color: rebeccapurple;
//      //animation: animation2 80s linear infinite;
//      //animation-delay: -40s;
//  }
//
//
//
//
//
//  i {
//    color: #1e1e1e;
//  }
//
//  @keyframes animationx {
//    0% {
//      background-color: red;
//      transform: translateX(100%);
//    }
//    100% {
//      transform: translateX(-100%);
//    }
//  }
//
//  @keyframes animation2 {
//    0% {
//      background-color: rebeccapurple;
//      transform: translateX(100%);
//    }
//    100% {
//      transform: translateX(-100%);
//    }
//  }
//}


</style>