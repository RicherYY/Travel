<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="item in swiperList" v-bind:key="item.id">
        <img class="swiper-img" v-bind:src="item.imgUrl">
      </swiper-slide>
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
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [{
        id: '0001',
        imgUrl: 'https://source.qunarzz.com/site/images/wns/20190514_qunar_dujia_homepage_3.jpg'}, {
        id: '0002',
        imgUrl: 'https://source.qunarzz.com/site/images/wns/20190517_qunar_dujia_homepage_top_banner_1.jpg'}]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background : #fff !important
  .wrapper
    width : 100%
    height : 0
    overflow : hidden
    padding-bottom : 25.25%
    background : #eee
    .swiper-img
      width : 100%
</style>
