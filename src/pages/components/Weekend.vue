<template>
  <div>
    <div class="title">周末去哪儿</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl" >
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1811/15/66f14e0fd6fbb.jpg_r_640x214_5d69f21d.jpg',
        title: '东部华侨城大侠谷',
        desc: '5.27-6.2六一有优惠！点进来看呀~'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1811/15/66f14e0fd6fbb.jpg_r_640x214_5d69f21d.jpg',
        title: '东部华侨城大侠谷',
        desc: '5.27-6.2六一有优惠！点进来看呀~'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/source/1811/15/66f14e0fd6fbb.jpg_r_640x214_5d69f21d.jpg',
        title: '东部华侨城大侠谷',
        desc: '5.27-6.2六一有优惠！点进来看呀~'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import "~styles/mixins.styl"
  .title
    margin-top .2rem
    line-height .8rem
    background #eee
    text-indent .2rem
  .item-img-wrapper
    padding-bottom 33.9%
    height 0
    overflow hidden
    .item-img
      width 100%
  .item-info
    padding .1rem
    .item-title
      font-size .32rem
      line-height .54rem
      ellipsis()
    .item-desc
      line-height .4rem
      color #ccc
      ellipsis()
</style>
