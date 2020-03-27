<template>
    <section class="msite">
        <HeaderTop title="地址">
         <router-link class="header_search" slot="left" >
         </router-link>
         <router-link class="header_login" slot="right">
             <span>
                  登录|注册
             </span>
         </router-link>
        </HeaderTop>
        <div class="mister-content-wrapper">
            <div class="miste-content">
               <nav class="msite_nav"></nav> 
            </div>
        </div>
    </section>
</template>

<script>
  import HeaderTop from '../../components/HeaderTop.vue'
  

export default {
  data () {
      return {
        address: "地址"
      }
    },
  components: {
      HeaderTop,
    }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
   .msite
     width 100%
     background-color gray 
     .msite-content-wrapper
       background-color yellow
       position fixed
       top 45px
       left 0px
       right 0px
       bottom 46px
       width 100%
       .msite_nav
         bottom-border-1px(#e4e4e4)
         margin-top 15px
         height 200px
         background-color green

 
</style>

