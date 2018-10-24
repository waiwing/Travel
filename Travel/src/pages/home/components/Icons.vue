<template>
  <div class="icons">
    <swiper>
      <swiper-slide v-for="(pageItemList, index) of pages" :key="index">
        <div class="icon" v-for="item of pageItemList" :key="item.id">
          <div class="icon-img">
            <img class="icon-img-content" :src="item.imgUrl"/>
          </div>
          <p class="icon-desc">{{item.descL}}</p>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeIcons',
  data: () => {
    return {
      iconList: [{
        id: '1001',
        imgUrl: '../../../assets/img/jingdian.png',
        descL: '好地方'
      }, {
        id: '1002',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1002',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1002',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1002',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1002',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1002',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1002',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1002',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1002',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1002',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }, {
        id: '1002',
        imgUrl: '../../../assets/img/jingdian2.png',
        descL: '老地方'
      }]
    }
  },
  computed: {
    pages () {
      const pages = []
      this.iconList.forEach((element, index) => {
        const page = Math.floor(index / 8)
        if (!pages[page]) {
          pages[page] = []
        }
        pages[page].push(element)
      })
      return pages
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  @import '~styles/mixins.styl'

  .icons >>> .swiper-container
     height 0
     padding-bottom 50%
    .icon
      position relative
      overflow hidden
      float left
      width 25%
      height 0
      padding-bottom 25%
      .icon-img
        position absolute
        top 0
        left 0
        right 0
        bottom .44rem
        box-sizing border-box
        padding .1rem
      .icon-img-content
        height 100%
        display block
        margin 0 auto
    .icon-desc
      position absolute
      left 0
      right 0
      bottom 0
      height .44rem
      line-height .44rem
      ellipsis()
</style>
