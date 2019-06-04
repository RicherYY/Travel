<template>
  <ul class="list">
    <li class="item">A</li>
    <li class="item">A</li>
    <li class="item">A</li>
    <li class="item">A</li>
    <li class="item">A</li>
  </ul>
</template>

<script>
export default {
  name: 'CityAlphabet'
}
</script>

<style lang="stylus" scoped>
  .list
    display flex
    flex-direction column
    justify-content center
    top 1.58rem
    right 0
    bottom 0
    width .4rem
    position absolute
    .item
      color $bgColor
      text-align center
      line-height .44rem
</style>
