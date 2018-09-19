<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item">
        <div class="item-img-wraper">
          <img src="http://img1.qunarzz.com/sight/p0/1705/99/99cad7081abb9771a3.img.jpg_200x200_d86753f0.jpg" class="item-img">
        </div>
        <div class="info">
          <p class="item-title">武汉九峰森林动物园</p>
          <p class="item-desc">
            <span class="star">★★★★☆</span>
            <span class="comment">806条评论</span>
          </p>
          <p class="item-price">
            <span class="price">$18</span>起
            <span class="address">江岸区</span>
          </p>
          <p class="pome">一所老屋，一段故事，一种悠哉的慢生活</p>
        </div>
      </li>
      <li class="item">
        <div class="item-img-wraper">
          <img src="http://img1.qunarzz.com/sight/p0/1705/99/99cad7081abb9771a3.img.jpg_200x200_d86753f0.jpg" class="item-img">
        </div>
        <div class="info">
          <p class="item-title">武汉九峰森林动物园</p>
          <p class="item-desc">
            <span class="star">★★★★☆</span>
            <span class="comment">806条评论</span>
          </p>
          <p class="item-price">
            <span class="price">$18</span>起
            <span class="address">江岸区</span>
          </p>
          <p class="pome">一所老屋，一段故事，一种悠哉的慢生活</p>
        </div>
      </li>
      <li class="item">
        <div class="item-img-wraper">
          <img src="http://img1.qunarzz.com/sight/p0/1705/99/99cad7081abb9771a3.img.jpg_200x200_d86753f0.jpg" class="item-img">
        </div>
        <div class="info">
          <p class="item-title">武汉九峰森林动物园</p>
          <p class="item-desc">
            <span class="star">★★★★☆</span>
            <span class="comment">806条评论</span>
          </p>
          <p class="item-price">
            <span class="price">$18</span>起
            <span class="address">江岸区</span>
          </p>
          <p class="pome">一所老屋，一段故事，一种悠哉的慢生活</p>
        </div>
      </li>
      <li class="item">
        <div class="item-img-wraper">
          <img src="http://img1.qunarzz.com/sight/p0/1705/99/99cad7081abb9771a3.img.jpg_200x200_d86753f0.jpg" class="item-img">
        </div>
        <div class="info">
          <p class="item-title">武汉九峰森林动物园</p>
          <p class="item-desc">
            <span class="star">★★★★☆</span>
            <span class="comment">806条评论</span>
          </p>
          <p class="item-price">
            <span class="price">$18</span>起
            <span class="address">江岸区</span>
          </p>
          <p class="pome">一所老屋，一段故事，一种悠哉的慢生活</p>
        </div>
      </li>
      <li class="item">
        <div class="item-img-wraper">
          <img src="http://img1.qunarzz.com/sight/p0/1705/99/99cad7081abb9771a3.img.jpg_200x200_d86753f0.jpg" class="item-img">
        </div>
        <div class="info">
          <p class="item-title">武汉九峰森林动物园</p>
          <p class="item-desc">
            <span class="star">★★★★☆</span>
            <span class="comment">806条评论</span>
          </p>
          <p class="item-price">
            <span class="price">$18</span>起
            <span class="address">江岸区</span>
          </p>
          <p class="pome">一所老屋，一段故事，一种悠哉的慢生活</p>
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
  ul {
    list-style: none;
    padding: 0;
    padding-left: .2rem;
  }
  .title {
    line-height: .8rem;
    background-color: #eee;
    text-align: left;
    padding-left: 4%;
    font-size: .3rem;
  }
  .item {
    position: relative;
    display: flex;
    height: 1.9rem;
    margin-bottom: .90rem;
  }
  .item::after {
    content: '';
    position: absolute;
    display: block;
    width: 100%;
    height: 1px;
    border-bottom: 1px solid #eee;
    bottom: -0.8rem;
    left: -0.1rem;
  }
  .item .item-img-wraper {
    width: 2rem;
    height: 2rem;
    display: flex;
    justify-content:center;
    align-items: center;
  }
  .item .item-img-wraper img {
    width: 90%;
  }
  .item p {
    margin: 0;
    padding: 0;
    padding-left: .1rem;
    line-height: .44rem;
    height: .44rem;
  }
  .item .info {
    flex: 1;
  }
  .info .item-title {
    margin-top: .28rem;
  }
  .info .item-desc {
    margin-top: .08rem;
    color: #ffb436;
    font-size: .25rem;
  }
  .info .item-price {
    margin-top: .1rem;
    font-size: .25rem;
    position: relative;
    color: #616161;;
  }
  .info .item-price .price {
    font-size: .42rem;
    color: #ff8300;
  }
  .info .item-price .address {
    position: absolute;
    right: .28rem;
  }
  .info .pome {
    margin-top: .3rem;
    font-size: .22rem;
    color: #f55;
  }
</style>
