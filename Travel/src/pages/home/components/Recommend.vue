<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="(item) of recommendList"  :key="item.id">
        <img  class="item-img" src="../../../assets/img/jingdian.png"/>
        <div class="item-info">
          <p class="item-title">{{item.descL}}</p>
          <p class="item-desc">{{item.descL}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data: () => {
    return {
      recommendList: [{
        id: '1001',
        imgUrl: '../../../assets/img/jingdian.png',
        descL: '好地方'
      }, {
        id: '1002',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1003',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1004',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1005',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1006',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1007',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1008',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1009',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1010',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1011',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1012',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'

  .title
    margin-top .2rem
    line-height .8rem
    background #eee
    text-indent .2rem
  .item
    display flex
    height 1.9rem
    overflow hidden
    .item-img
       width 1.7rem
       height 1.7rem
       padding .1rem
    .item-info
       flex 1
       padding .1rem
       text-align left
       min-width 0
       .item-title
          line-height .54rem
          font-size .32rem
          ellipsis()
       .item-desc
          line-height .4rem
          color #ccc
          ellipsis()
       .item-button
          margin-left .44rem
          margin-top .2rem
          background #ff9300
          padding 0.1rem
          border-radius .06rem
          color #fff

</style>
