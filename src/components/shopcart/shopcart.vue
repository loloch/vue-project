<template>
  <div>
    <div class="cartheader">
      <span class="cartexit"></span>
      <span class="headertitle">购物车</span>
    </div>
    <div class="cartcontent">
      <div class="login">
        <a class="loginbtn" href="javascript:;">登录</a>
        <span class="loginpro">在登录之后您可以同步电脑与手机中的购买商品</span>
      </div>
      <div class="scorechangewrap">
        <div class="scorechange">
          <input class="changeinput" type="text">
          <input class="changebtn" type="btn" value="兑换">
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default{
    components: {
    }
  }
</script>

<style lang='stylus' rel='stylesheet/stylus'>
  .cartheader
    width 100%
    height 4rem
    line-height 4rem
    background-color #89be48
    position fixed
    left 0
    top 0
    .cartexit
      display inline-block
      height 4rem
      width 4rem
      background-image  url("./direct.png")
      background-repeat no-repeat
      background-position 40%
      background-size 35%
    .headertitle
      display inline-block
      position absolute
      left 155px
      top 0
      color white
      font-size 2rem
  .cartcontent
    padding-top 4rem
    .login
      height 3rem
      line-height 3rem
      padding-top 4px
      background-color: #f0fae6;
      .loginbtn
        width: 18%;
        height: 2.6rem;
        border-radius 2px
        display: inline-block;
        background: #fff;
        border: 1px solid #8bc146;
        text-align: center;
        font-size: 1.5rem;
        color: #88c13e;
        line-height: 2.5rem;
        margin 0 10px
      .loginpro
        display: inline-block;
        font-size: 1.2rem;
        color: #333;


  .scorechangewrap
    width: 100%;
    height: 3.2rem;
    background-color: #fff;
    padding: .6rem 0 .5rem;
    border-bottom: 1px solid #f2f2f2;
    .scorechange
      width: 100%;
      height: 3.2rem;
      background-color: #fff;
      margin: 0;
      padding: .6rem 0 .5rem;
      border-bottom: 1px solid #f2f2f2;
      .changeinput
        padding-left: 10px;
        width: 80%;
        height: 2.8rem;
        line-height: 2.8rem;
        display: inline-block;
        border-radius: 0;
        border: 1px solid #e7e7e7;
        background: #fff;
        text-align: left;
        font-size: 1.4rem;
        outline 0 none
      .changebtn
        width: 20%;
        height: 3rem;
        line-height: 3rem;
        display: inline-block;
        border-radius: 0;
        background: #fff;
        text-align: center;
        font-size: 1.6rem;
        color: #6fbd00;
        letter-spacing: .1rem;
        text-indent: .2rem;
        position: absolute;
        right: 0;
        top: 0;
        z-index: 3;
        border: 1px solid #6fbd00;
</style>
