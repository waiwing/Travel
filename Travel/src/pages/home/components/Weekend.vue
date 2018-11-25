<template>
  <div>
    <div class="title">周末</div>
    <ul>
      <li class="item border-bottom" v-for="(item) of recommendList"  :key="item.id">
       <div class="item-img-wrapper">
         <img  class="item-img" src="../../../assets/img/jingdian.png"/>
       </div>
        <div class="item-info">
          <p class="item-title">{{item.descL}}</p>
          <p class="item-desc">{{item.descL}}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
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
    .item-img-wrapper
      height 0
      overflow hidden
      padding-bottom 33.9%
      .item-img
        width 100%
    .item-info
        padding .1rem
     .item-title
        line-height .54rem
        font-size .32rem
        ellipsis()
      .item-desc
        line-height .4rem
        color #ccc
        ellipsis()

</style>
