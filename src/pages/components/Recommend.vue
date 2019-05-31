<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl" >
        </div>
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1502/15/15ca1d0eab6bf46c.water.jpg_200x200_50ca7bb1.jpg',
        title: '东部华侨城大侠谷',
        desc: '5.27-6.2六一有优惠！点进来看呀~'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1905/98/980c6d998016cc67a3.water.jpg_200x200_9965e349.jpg',
        title: '东部华侨城大侠谷',
        desc: '5.27-6.2六一有优惠！点进来看呀~'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1508/2e/d9363ce50a88c8c5ff5a138c67687cd4.water.jpg_200x200_1c15c8f5.jpg',
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
.item
  overflow hidden
  display flex
  height 1.9rem
  .item-img
    padding .1rem
    height 1.7rem
    width 1.7rem
  .item-info
    flex 1
    padding .1rem
    min-width 0
    .item-title
      font-size .32rem
      line-height .54rem
      ellipsis()
    .item-desc
      line-height .4rem
      color #ccc
      ellipsis()
    .item-button
      line-height .44rem
      color #fff
      margin-top .16rem
      border-radius .06rem
      background #ff9300
      padding 0 .2rem
</style>
