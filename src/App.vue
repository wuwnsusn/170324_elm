<template>
  <div>
    <elm-header></elm-header>
    <div class='tab'>
      <div class="tab-item">
        <router-link to='/goods'>商品</router-link>
      </div>
      <div class="tab-item">
        <router-link to='/ratings'>评价</router-link>
      </div>
      <div class="tab-item">
        <router-link to='/seller'>商家</router-link>
      </div>

    </div>
    <router-view></router-view>
  </div>
</template>

<script>
  import header from './components/header/header.vue'
  export default {
    components:{
      'elm-header':header
    }
  }
</script>

<style lang='stylus' rel='stylesheet/stylus'>
  @import './common/styuls/mixin.styl'
/*商品、评价、商家 用flex布局写*/
  .tab
    display flex
    height 40px
    line-height 40px
    border-1px(rgba(7,17,27,.1))
    .tab-item
      font-size 14px
      width 0
      flex 1
      text-align center
      &>a
        display block
        color rgb(77,85,93)
        &.active
          color rgb(240,20,20)

</style>
