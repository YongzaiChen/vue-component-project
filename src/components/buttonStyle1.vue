<template>
  <div id="buttonStyle1">
    <span>{{ name }}</span>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      default: ""
    }
  }
}
</script>


<style scoped>
#buttonStyle1 span {
  display: inline-block;
  background: linear-gradient(to right, #3b91ff, #3b91ff) no-repeat left bottom;
  background-size: 0px 3px;
  transition: background 0.25s;
  padding-bottom: 4px;
  font-size: 14px;
  user-select: none;
  cursor: pointer;
}

#buttonStyle1:hover {
  color: #3b91ff;
}

#buttonStyle1 span:hover {
  display: inline-block;
  background: linear-gradient(to right, #3b91ff, #3b91ff) no-repeat left bottom;
  background-size: 100% 3px;
  padding-bottom: 4px;
}
</style>