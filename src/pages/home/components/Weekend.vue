<template lang="html">
  <div class="">
    <div class="title">周末去哪</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <div class="item-img-wrapper">
          <img class="item-img" :src="item.imgUrl">
        </div>
        <div class="item-info">
          <p class="item-title">{{ item.title }}</p>
          <p class="item-desc">{{ item.desc }}</p>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      recommendList: [
        {
          id: '0001',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1505/c2/0be94f64d9df91.jpg_r_640x214_130f7614.jpg',
          title: '当当城儿童职业体验馆',
          desc: '[周末/节假日]御龙温泉成人票（含水上乐园）'
        }, {
          id: '0002',
          imgUrl: 'http://img1.qunarzz.com/sight/source/1505/c2/0be94f64d9df91.jpg_r_640x214_130f7614.jpg',
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
  .item-img-wrapper
    overflow: hidden
    height: 0
    padding-bottom: 33.9%
    .item-img
      width: 100%
  .item-info
    padding: .1rem
    .item-title
      line-height: .48rem
      font-size: .28rem
      ellipsis()
    .item-desc
      line-height: .3rem
      color: #ccc
      ellipsis()
</style>
