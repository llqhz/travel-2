<template>
  <div class="icons">
    <swiper>
      <swiper-slide v-for="(page,index) in pages" :key='index'>
        <div class="icon" v-if="index<8" v-for="(item,index) in page" :key="item.id">
            <img :src="item.src" >
            <p>{{ item.title }}</p>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
export default {

}
</script>


