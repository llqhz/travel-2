<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe628;</div>
    </div>
    <div class="header-center">
      <span class="iconfont">&#xe648;</span>
      &nbsp; 输入城市/景点/游玩主题
    </div>
    <div class="header-right">
      城市
      <span class="iconfont">&#xe652;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style scoped>
  .header {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-between;
    align-items: center;
    align-content: center;

    background-color: #00bcd4;
    height: .86rem;
  }
  .back-icon {
    text-align: center;
    font-size: .4rem;
    font-weight: bold;
  }
  .header-left,.header-right {
    margin: .2rem;
    color: #fff;
    text-align: center;
  }
  .header-center {
    flex-grow: 1;
    display: flex;
    align-items: center;

    background-color: #fff;
    border-radius: .08rem;
    height: .65rem;
    color: #ccc;

    padding-left: .2rem;
  }

</style>
