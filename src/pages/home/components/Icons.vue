<template>
  <div class="icons">
    <swiper :options="swiperOption">
      <swiper-slide v-for="(page,index) in pages" :key='index'>
        <div class="icon" v-if="index<8" v-for="(item,index) in page" :key="item.id">
            <img :src="item.src" >
            <p>{{ item.title }}</p>
        </div>
      </swiper-slide>
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeIcons',
  data: () => {
    return {
      swiperOption: {
        loop: true,
        autoplay: 3000,
        pagination: '.swiper-pagination'
      },
      icons: [
        {
          id: 1,
          title: '景点门票',
          src: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png'
        },
        {
          id: 2,
          title: '武汉必游',
          src: 'http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png'
        },
        {
          id: 3,
          title: '游乐场',
          src: 'http://img1.qunarzz.com/piao/fusion/1803/95/8246f27355943202.png'
        },
        {
          id: 4,
          title: '夏日玩水游山玩水很好玩',
          src: 'http://img1.qunarzz.com/piao/fusion/1803/6a/45f595250c73d102.png'
        },
        {
          id: 5,
          title: '海洋馆',
          src: 'http://img1.qunarzz.com/piao/fusion/1803/50/26ffa31b56646402.png'
        },
        {
          id: 6,
          title: '一日游',
          src: 'http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png'
        },
        {
          id: 7,
          title: '名胜古迹',
          src: 'http://img1.qunarzz.com/piao/fusion/1803/20/831d62d2e1c7be02.png'
        },
        {
          id: 8,
          title: '武汉欢乐谷',
          src: 'http://img1.qunarzz.com/piao/fusion/1803/b1/528a9e80403b8c02.png'
        },
        {
          id: 9,
          title: '水上玩乐',
          src: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png'
        },
        {
          id: 10,
          title: '全部玩乐',
          src: 'http://img1.qunarzz.com/piao/fusion/1803/80/416c6ab3368d1f02.png'
        }

      ]
    }
  },
  computed: {
    pages: function () {
      let pages = []
      this.icons.forEach((item, index) => {
        let page = Math.floor(index / 8)
        if (!pages[page]) {
          pages.push([])
        }
        pages[page].push(item)
      })
      return pages
    }
  }
}
</script>

<style scoped>
  /* 只起占位作用 */
  .icons >>> .swiper-container {
    height: 0;
    width: 100%;
    padding-bottom: 50%;
    overflow: hidden;
    background-color: #fff;
  }
  .icons >>> .swiper-pagination {
    bottom: -2%;
  }
  .icons {
    margin-top: .2rem;
    margin-bottom: .2rem;
  }
  .icons >>> .swiper-slide {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: flex-start;
    align-items: flex-start; /* 子项目基线对齐方式 */
    align-content: flex-start;
  }
  .icon {
    width: 25%;
    height: 0;
    overflow: hidden;
    padding-bottom: 25%;
    /* border: 1px solid red; */
    box-sizing: border-box;
    margin: 0;

    display: flex;
    flex-flow: row wrap;
    justify-content: center;
    align-items: center;
    align-content: flex-start;

    flex-wrap: wrap;
  }
  .icon img {
    margin-top: 10%;
    width: 60%;
    display: block;
  }
  .icon p {
    width: 100%;
    text-align: center;

    margin: 0;
    color: #212121;
    font-size: .25rem;

    /* 单行文本 多余字省略号 */
    overflow: hidden;
    white-space: nowrap;
    text-overflow: ellipsis;
  }

</style>
