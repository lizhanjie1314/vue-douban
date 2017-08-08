<template>
  <div id="navFooter" class="navFooter">
    <h2><a href="javascript:;">{{msg}}</a></h2>

  </div>
</template>
<script>
  export default{
      data(){
          return{
              msg:"登陆"
          }
      }
  }
</script>
<style scoped>
  a{
    display: block;
    width: 6rem;
    height: 3.4rem;
    line-height: 3.4rem;
    font-size: 1.4rem;
    background: #3385ff;
    color: #fff;
    text-align: center;
    margin: 0 auto;
    cursor: pointer;
  }


</style>
