<template>
  <div id="app">
    <v-header></v-header>
    <div class="tab border-1px">
       <div class="tab-item">商品</div>
       <div class="tab-item">评论</div>
       <div class="tab-item">商家</div>
    </div>
    <div class="content">
        I am content
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
  import header from './components/header/header.vue';
  export default {
    components: {
      'v-header': header
    }
  };
</script>

<style lang="stylus" rel="stylesheet/stylus">
  #app
  .tab
      display: flex
      width: 100%
      height: 40px
      line-height: 40px
      border-bottom: 1px solid rgba(7, 17, 27, 0.1)
      .tab-item
        flex: 1
        text-align: center
        & > a
          display: block
          font-size: 14px
          color: rgb(77, 85, 93)
          &.active
            color: rgb(240, 20, 20)
</style>
