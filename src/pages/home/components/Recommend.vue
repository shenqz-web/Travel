<template lang="html">
  <div class="">
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl">
        </div>
        <div class="item-info">
          <p class="item-title">{{ item.title }}</p>
          <p class="item-desc">{{ item.desc }}</p>
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
      recommendList: [
        {
          id: '0001',
          imgUrl: 'https://imgs.qunarzz.com/sight/p0/1511/2e/2e3c8d254fdee61690.water.jpg_110x110_1fc9f714.jpg',
          title: '当当城儿童职业体验馆',
          desc: '[周末/节假日]御龙温泉成人票（含水上乐园）'
        }, {
          id: '0002',
          imgUrl: 'https://imgs.qunarzz.com/sight/p0/1511/2e/2e3c8d254fdee61690.water.jpg_110x110_1fc9f714.jpg',
          title: '当当城儿童职业体验馆',
          desc: '[周末/节假日]御龙温泉成人票（含水上乐园）'
        }, {
          id: '0003',
          imgUrl: 'https://imgs.qunarzz.com/sight/p0/1511/2e/2e3c8d254fdee61690.water.jpg_110x110_1fc9f714.jpg',
          title: '当当城儿童职业体验馆',
          desc: '[周末/节假日]御龙温泉成人票（含水上乐园）'
        }, {
          id: '0004',
          imgUrl: 'https://imgs.qunarzz.com/sight/p0/1511/2e/2e3c8d254fdee61690.water.jpg_110x110_1fc9f714.jpg',
          title: '当当城儿童职业体验馆',
          desc: '[周末/节假日]御龙温泉成人票（含水上乐园）'
        }, {
          id: '0005',
          imgUrl: 'https://imgs.qunarzz.com/sight/p0/1511/2e/2e3c8d254fdee61690.water.jpg_110x110_1fc9f714.jpg',
          title: '当当城儿童职业体验馆',
          desc: '[周末/节假日]御龙温泉成人票（含水上乐园）'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-indent: .2rem
  .item
    display: flex
    height: 1.9rem
    margin: .1rem 0
    overflow: hidden
    .item-img
      width: 1.7rem
      height: 1.7rem
      padding: .1rem
    .item-info
      flex: 1
      padding: .1rem
      min-width: 0
      .item-title
        line-height: .54rem
        font-size: .32rem
        ellipsis()
      .item-desc
        line-height: .4rem
        color: #ccc
        ellipsis()
      .item-button
        margin-top: .2rem
        background: #ff9300
        padding: .05rem .2rem
        border-radius: .06rem
        color: #fff
</style>
