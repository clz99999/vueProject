<!--首页黑色按钮：黑色背景白色字  hover效果：透明背景黑色字黑色边框-->
<template>
  <div>
    <button>{{text}}</button>
  </div>
</template>

<script>
  export default{
    name: '',
    data: function () {
      return {}
    },
    props:['text']
  }
</script>

<style scoped lang="less">
  @import "../../assets/css/common.less";
  button{
    width: 176px;
    height: 40px;
    background-color: @mainblack;
    color: @bgwhite;
    font-size: @mainfontsize;
    outline: none;
    border: 1px solid @mainblack;
    transition: all 0.3s;
  }
  button:hover{
    background-color: transparent;
    color: @mainblack;
    transition: all 0.3s;
  }
</style>
