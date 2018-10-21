<template>
  <div class="wrapper">
    <swiper :options="swiperOption" >
      <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl"/>
      </swiper-slide>

      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>

</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [
        {
          id: '0001',
          imgUrl: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1540134472253&di=d823d4335e38a6dff9c7345fff548e49&imgtype=0&src=http%3A%2F%2Fimg.weixinyidu.com%2F160317%2Fb0a17d30.jpg'
        }, {
          id: '0002',
          imgUrl: 'https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1540134472251&di=fc66182af469d1560d43463e872b5d26&imgtype=0&src=http%3A%2F%2Fm.tuniucdn.com%2Ffilebroker%2Fcdn%2Folv%2F40%2F68%2F40689ab62aac7b5a21426e3e0a7fbd11_w800_h0_c0_t0.jpg'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>

  .wrapper
    overflow  hidden
    width 100%
    height 0
    padding-bottom 31.25%
    background grey
  .swiper-img
    width 100%
</style>
