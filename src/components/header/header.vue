<template>
  <div class='header'>
    <div class="content-wrapper">
      <!--内容包装-->
      <div class="avatar">
        <img src="http://static.galileo.xiaojukeji.com/static/tms/seller_avatar_256px.jpg" width='64' height='64'>
      </div>
      <div class="content">
        <div class="title">
          <span class='brand'></span>
          <span class='name'>粥品香坊（回龙观）</span>
        </div>
        <div class="description">蜂鸟专送/38分钟送达</div>
        <div class="supports">
          <span class='icon decrease'></span>
          <span class="text">在线支付 满20送可乐</span>
        </div>
      </div>
      <div class="supports-count">
        <span class="count">5个</span>
        <span class="icon-keyboard_arrow_right"></span>
      </div>
    </div>
    <div class="bulletin-wrapper">
      <!--公告包装-->
      <span class="bulletin-title"></span>
      <span class="bulletin-text">
        粥品香坊其烹饪粥料的秘方源于中国千年古法，在融和现代制作工艺，由世界烹饪大师屈浩先生领衔研发。坚守纯天然、0添加的良心品质深得消费者青睐，发展至今成为粥类的引领品牌。是2008年奥运会和2013年园博会指定餐饮服务商。
      </span>
      <span class="icon-keyboard_arrow_right"></span>
    </div>
    <div class="background">
      <!--header背景模糊图-->
      <img src="http://static.galileo.xiaojukeji.com/static/tms/seller_avatar_256px.jpg" width="100%" height="100%">
    </div>
    <div class="mask">
      <!--遮罩区域-->
      <div class="mask-wrapper clearfix">
        <div class="mask-main">
          <h1 class="title">粥品香坊(平西王府）</h1>
          <div class="star-wrapper">
            <div class="stars stars-48">
              <spam class="star on"></spam>
              <spam class="star on"></spam>
              <spam class="star on"></spam>
              <spam class="star half"></spam>
              <spam class="star off"></spam>
            </div>
          </div>
          <div class="info">
            <div class="line"></div>
            <div class="text">优惠信息</div>
            <div class="line"></div>
          </div>
          <ul class="list">
            <li class="item">
              <span class="icon decrease"></span>
              <span class="text">在线支付满10送2个小公仔</span>
            </li>
            <li class="item">
              <span class="icon discount"></span>
              <span class="text">VC无限橙果汁全场8折</span>
            </li>
            <li class="item">
              <span class="icon guarantee"></span>
              <span class="text">单人精彩套餐</span>
            </li>
            <li class="item">
              <span class="icon invoice"></span>
              <span class="text">该商家支持发票,请下单写好发票抬头</span>
            </li>
            <li class="item">
              <span class="icon special"></span>
              <span class="text">已加入“外卖保”计划,食品安全保障</span>
            </li>
          </ul>
          <div class="info">
            <div class="line"></div>
            <div class="text">商家公告</div>
            <div class="line"></div>
          </div>
          <div class="bulletin">
            <span class="text">
              粥品香坊其烹饪粥料的秘方源于中国千年古法，在融和现代制作工艺，由世界烹饪大师屈浩先生领衔研发。坚守纯天然、0添加的良心品质深得消费者青睐，发展至今成为粥类的引领品牌。是2008年奥运会和2013年园博会指定餐饮服务商。
            </span>
          </div>
        </div>
      </div>
      <div class="mask-footer">
        <span class="icon-close"></span>
      </div>
    </div>
  </div>
</template>

<script>
  export default {}
</script>

<style lang='stylus' rel='stylesheet/stylus'>
  @import '../../common/styuls/mixin.styl'

  .header
    position relative
    color #fff
    background-color rgba(7, 17, 27, .5)
    overflow hidden
    .content-wrapper
      position relative
      padding 24px 12px 18px 24px
      font-size 0
      .avatar
        display inline-block
        vertical-align top
      .content
        display inline-block
        margin-left 16px
        .title
          margin 2px 0 8px 0
          .brand
            display inline-block
            width 30px
            height 18px
            bg-image(brand)
            background-size 30px 18px
            background-repeat no-repeat
            vertical-align top
            /*background-image: url(brand@2x.png);
            background-image: url(brand@3x.png);*/
          .name
            margin-left 6px
            font-size 16px
            font-weight bold
            line-height 18px
        .description
          font-size 12px
          line-height 12px
          font-weight 200
        .supports
          margin 10px 0 2px 0
          .icon
            display: inline-block
            width: 12px
            height: 12px
            background-size 12px 12px
            background-repeat no-repeat
            vertical-align top
            &.decrease
              bg-image(decrease_1)
            &.discount
              bg-image(discount_1)
            &.guarantee
              bg-image(guarantee_1)
            &.invoice
              bg-image(invoice_1)
            &.special
              bg-image(special_1)
          .text
            margin-left 4px
            font-size 10px
            line-height 12px
            font-weight 200


      .supports-count
        position absolute
        right 12px
        bottom 15px
        height 10px
        line-height 10px
        padding 7px 8px
        border-radius 10px
        background-color rgba(0,0,0,.2)
        .count
          font-size 10px
          line-height 10px
          font-weight 200
          margin-right 2px
        .icon-keyboard_arrow_right
          font-size 10px
          line-height 10px
          font-weight 200

    .bulletin-wrapper
      position relative
      overflow: hidden
      white-space nowrap
      text-overflow ellipsis
      padding 0 22px 0 12px
      background-color rgba(7, 17, 27, .2)
      .bulletin-title
        display: inline-block
        width: 22px
        height: 12px
        vertical-align top
        margin-top 7px
        background-size 22px 12px
        background-repeat no-repeat
        bg-image(bulletin)
      .bulletin-text
        font-size 10px
        line-height 28px
        font-weight: 200
      .icon-keyboard_arrow_right
        /*main.js 里引用index.styl 引入了icon.styl，icon-keyboard_arrow_right才会生效 */
        position absolute
        right 12px
        bottom 0
        font-size 10px
        line-height 28px
        font-weight 200


    .background
      position absolute
      left 0
      top 0
      filter blur(10px)
      z-index -1
      width 100%
      height 100%
    .mask
      display: none
      position fixed
      z-index 100
      left 0
      top 0
      width 100%
      height 100%
      overflow: auto
      background rgba(7, 17, 27, .8)
      .mask-wrapper
        min-height 100%
        .mask-main
          padding 64px 32px
          .title
            font-size 16px
            font-weight 700
            line-height 16px
            text-align center
          .star-wrapper
            padding 16px 0 0 0
            height 24px
            .stars
              height 24px
              text-align center
              .star
                display: inline-block
                background-repeat no-repeat
              &.stars-36
                .star
                  margin-right 12px
                  width 15px
                  height 15px
                  background-size 15px 15px
                  &:last-child
                    margin-right 0px
                  &.on
                    bg-image("../star/star36_on")
                  &.half
                    bg-image("../star/star36_half")
                  &.off
                    bg-image("../star/star36_off")
              &.stars-24
                .star
                  margin-right 10px
                  width 10px
                  height 10px
                  background-size 10px 10px
                  &:last-child
                    margin-right 0px
                  &.on
                    bg-image("../star/star24_on")
                  &.half
                    bg-image("../star/star24_half")
                  &.off
                    bg-image("../star/star24_off")
              &.stars-48
                .star
                  margin-right 15px
                  width 20px
                  height 19px
                  background-size 20px 19px
                  &:last-child
                    margin-right 0
                  &.on
                    bg-image('../star/star48_on')
                  &.half
                    bg-image('../star/star48_half')
                  &.off
                    bg-image('../star/star48_off')
          .list
            .item
              margin-bottom 12px
              .icon
                display: inline-block
                width 16px
                height 16px
                -webkit-background-size 16px 16px
                background-size 16px 16px
                background-repeat no-repeat
                vertical-align middle
                &.decrease
                  bg-image(decrease_2)
                &.discount
                  bg-image(discount_2)
                &.guarantee
                  bg-image(guarantee_2)
                &.invoice
                  bg-image(invoice_2)
                &.special
                  bg-image(special_2)
              .text
                font-size 12px
                line-height 12px
                font-weight 200
          .info
            display: flex
            margin 28px auto 24px auto
            .text
              margin 0 12px
              font-size 14px
              font-weight 700
              line-height 14px
            .line
              position relative
              top 7px
              flex 1
              height 1px
              background-color rgba(255,255,255,.2)
          .bulletin
            margin 0 12px
            .text
              font-size 12px
              font-weight 200
              line-height 24px
      .mask-footer
        margin-top -64px
        text-align center
        .icon-close
          font-size 32px
          color rgba(255,255,255,.5)

</style>
