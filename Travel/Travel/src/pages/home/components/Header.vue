<template>
  <div class="header">
    <div class="header-left">
        <div class="iconfont iconjiantou-px- back-icon"></div>
    </div>
    <div class="header-input">
        <span class="iconfont iconsousuo-px-"></span>
        输入城市/地点/内容
    </div>
    <router-link to='/city'>
      <div class="header-right">
          {{this.city}}
          <span class="iconfont iconjiantou arrow-icon"></span>
      </div>
    </router-link>
  </div>
</template>

<script>
export default{
  name: 'HomeHeader',
  props: {
    city: String
  }
}
</script>

<style lang="stylus" scoped>
   @import '~styles/varibles.styl'
  .header
    display: flex
    line-height: .86rem
    background: $bgColor
    color: #fff
    .header-left
      width: .64rem
      float: left
      .back-icon
        text-align: center
        font-size: .4rem
    .header-input
      flex: 1
      height: .64rem
      line-height: .64rem
      margin-top: .12rem
      margin-left: .2rem
      padding-left: .2rem
      background: #fff
      border-radius: .1rem
      color: #ccc
    .header-right
      width: 1.24rem
      float: right
      text-align: center
      color: #fff
      .arrow-icon
        margin-left: -.04rem
        font-size: .24rem
</style>
