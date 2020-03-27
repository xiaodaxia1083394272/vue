<template>
  <header class="header">
    <slot name="left"></slot>
    <span class="header_title">
      <span class="header_title_text ellipsis">{{title}}</span>
    </span>
    <slot name="right"></slot>
  </header>
</template>

<script>
export default {
  props:{
    title:String
  }    

}
</script>


<style lang="stylus" rel="stylesheet/stylus">
  .header
    background-color #02a774
    position fixed
    z-index 100
    left 0
    top 0
    width 100%
    height 45px
    .header_search
       background-color red
       position obsolute
       left 15px
       top 50%
       width 30px
       height 50px
    .header_title
       position absolute
       top 50%
       left 50%
       width 50%
       color yellow
       display block
    .header_login
       font-size 14px
       color #ffffff
       position absoulute
       right 15px
       top 50%
       
</style>



