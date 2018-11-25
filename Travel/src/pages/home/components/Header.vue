<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      请输入你要搜索的东西</div>
    <div class="header-right">
      <span class="iconfont">&#xe6aa;</span>
      {{this.city}}</div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  props: {
    city: String
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .header
    display: flex
    height: .86rem
    line-height: .86rem
    background: $bgColor
    color: #fff
    .header-left
      width: .64rem
      .back-icon
        text-align: center
        font-size:.4rem
    .header-input
      flex: 1
      background: #fff
      border-radius: .1rem
      margin-top: .12rem
      line-height : .64rem
      padding-left :.2rem
      height : .64rem
      margin-left .2rem
      color: #ccc
    .header-right
      width: 1.24rem
      text-align: center
</style>
