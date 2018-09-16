<!-- The ref attr used to find the swiper instance -->
<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="img in imgs" :key="img.id">
        <img :src="img.src" class="swipper-img">
      </swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        // some swiper options/callbacks
        // 所有的参数同 swiper 官方 api 参数
        // ...
        loop: true,
        autoplay: 3000,
        pagination: '.swiper-pagination'
      },
      imgs: [
        {
          id: 1,
          src: 'http://img1.qunarzz.com/piao/fusion/1806/ee/b889bce65d6dcf02.jpg_750x200_b1cb6a9f.jpg'
        },
        {
          id: 2,
          src: 'http://img1.qunarzz.com/piao/fusion/1808/74/cad6bf966300902.jpg_750x200_7641ba93.jpg'
        }
      ]

    }
  }
}
</script>

<style scoped>
  /* 设置图片占位宽高比 */
  .wrapper {
    width: 100%;
    height: 0;
    overflow: hidden;
    padding-bottom: 26.7%;
  }
  .wrapper .swipper-img {
    width: 100%;
  }
  /* 设置引用组件内的样式 */
  .wrapper >>> .swiper-pagination-bullet-active {
    background-color: white;
  }
</style>
