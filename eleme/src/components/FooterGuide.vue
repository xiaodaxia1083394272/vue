<template>
    <div class="footer_guide">
      <span class="guide_item" :class="{on: '/msite'===$route.path}" @click="goTo('/msite')">
          <span class="item_icon">
           <i class="iconfont icon-waimai"></i>
          </span>
          <span>首页</span>
      </span>
      <span class="guide_item" :class="{on: '/search'===$route.path}" @click="goTo('/search')">
          <span class="item_icon">
             <i class="iconfont icon-waimai"></i>
          </span>
          <span>搜索</span>
      </span>
      <span class="guide_item" :class="{on: '/order'===$route.path}" @click="goTo('/order')">
          <span class="item_icon">
             <i class="iconfont icon-waimai"></i>
          </span>
          <span>订单</span>
      </span>
      <span class="guide_item" :class="{on: '/profile'===$route.path}" @click="goTo('/profile')">
          <span class="item_icon">
             <i class="iconfont icon-waimai"></i>
          </span>
          <span>我的</span>
      </span>
    </div>
</template>

<script>
export default {
   methods: {
    //    跳转路由
      goTo (path) {
        //   console('路由点击')
        this.$router.replace(path)
      }
    } 
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
  @import "../common/stylus/mixins.styl"
   .footer_guide
      position fixed
      z-index 100
      left 0
      right 0
      bottom 0
      width 100%
      height 50px
      background-color green
      display flex
      .guide_item
         display flex
         flex 1//pss_水平且平分
         text-align center
         color #999999
         margin 5px
         flex-direction column
         background-color yellow
         align-items center
         &.on
           color #02a774
         span 
           font-size 12px
           margin-top 2px
           margin-bottom 2px
           .iconfont
              font-size 22px
 
</style>

