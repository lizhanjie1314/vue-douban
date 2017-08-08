<template>
  <div id="content" class="content">
    <nav-Head></nav-Head>
    <div class="swiper-container">
      <div class="swiper-wrapper">
        <div class="swiper-slide" v-for="item in swiperArr"><img :src='item'/></div>
        <!--<div class="swiper-slide" style="background: #4390EE;">Slide 1</div>-->
        <!--<div class="swiper-slide" style="background: #CA4040;">Slide 2</div>-->
        <!--<div class="swiper-slide" style="background: #FF8604;">Slide 3</div>-->
      </div>
      <!-- 如果需要分页器 -->
      <div class="swiper-pagination"></div>

      <!-- 如果需要导航按钮 -->
      <div class="swiper-button-prev"></div>
      <div class="swiper-button-next"></div>

      <!-- 如果需要滚动条 -->
      <!--<div class="swiper-scrollbar"></div>-->
    </div>
    <nav-Footer></nav-Footer>

  </div>
</template>
<script>
//  import Swiper from  '../../node_modules/swiper/dist/js/swiper.js'
//  import Swiper from
import navHead from "./navHead.vue";
import navFooter from "./navFooter.vue";
export default{
    components:{navHead,navFooter},
    data(){
        return{
            msg:"我是轮播",
          swiperArr:["../../static/1.jpg","../../static/2.jpg","../../static/3.jpg","../../static/4.jpg","../../static/5.jpg","../../static/6.jpg"]
        }
    },
   mounted(){
//        this.$nextTick(
     var mySwiper = new Swiper ('.swiper-container', {
       direction: 'horizontal',
       loop: true,
       autoplay : 5000,

       // 如果需要分页器
       pagination: '.swiper-pagination',
//
       // 如果需要前进后退按钮
       nextButton: '.swiper-button-next',
       prevButton: '.swiper-button-prev',

       // 如果需要滚动条
//       scrollbar: '.swiper-scrollbar',
     })
//   )
   }

}
</script>
<style>
  .swiper-container{margin-top: 4.8rem;}
  img{width: 100%;height: 100%;}
</style>
