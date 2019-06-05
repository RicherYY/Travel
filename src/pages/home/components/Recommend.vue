<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
        <router-link tag="li" class="item border-bottom" v-for="item of list" :key="item.id" :to="'/detail/' + item.id" >
          <div class="item-img-wrapper">
            <img class="item-img" :src="item.imgUrl" >
          </div>
          <div class="item-info">
            <p class="item-title">{{item.title}}</p>
            <p class="item-desc">{{item.desc}}</p>
            <button class="item-button">查看详情</button>
          </div>
        </router-link>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  props: {
    list: Array
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
