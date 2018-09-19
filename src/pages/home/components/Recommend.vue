<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item">
        <div class="item-img-wraper">
          <img src="" alt="" class="item-img">
        </div>
        <div class="info">
          <p class="item-title"></p>
          <p class="item-desc"></p>
          <p class="item-price"></p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend'
}
</script>

<style scoped>
  .title {
    line-height: .8rem;
    background-color: #eee;
    text-align: left;
    padding-left: 4%;
    font-size: .3rem;
  }
</style>
