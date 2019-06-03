<template>
    <div class="search">
      <input class="search-input" type="text" placeholder="输入城市名或拼音" />
    </div>
</template>

<script>
export default {
  name: 'Search'
}
</script>

<style lang="stylus" scoped>
  @import "~styles/varibles.styl"
  .search
    padding 0 .1rem
    background $bgColor
    height .72rem
    .search-input
      box-sizing border-box
      color #666
      border-radius .06rem
      text-align center
      width 100%
      line-height .62rem
      height .62rem
</style>
