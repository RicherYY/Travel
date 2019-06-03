<template>
    <div class="header">
      城市选择
      <router-link to="/">
        <div class="iconfont header-back">&#xe658;</div>
      </router-link>
    </div>
</template>

<script>
export default {
  name: 'CityHeader'
}
</script>

<style lang="stylus" scoped>
  @import "~styles/varibles.styl"
  .header
    position relative
    font-size .32rem
    background $bgColor
    color #fff
    text-align center
    line-height $headerHeight
    height $headerHeight
    overflow hidden
    .header-back
      color #fff
      position absolute
      top 0
      left 0
      font-size .4rem
      text-align center
      width .64rem
</style>
