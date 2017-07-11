<template>
  <div class="allgoods">
    <commonheader :con="con"></commonheader>
    <div class="goodsearch">
        <!--<mt-search-->
          <!--cancel-text="取消"-->
          <!--placeholder="搜索">-->
        <!--</mt-search>-->
      <form >
        <input type="text" class="searchinput" placeholder="搜索商品">
      </form>

    </div>

    <div class="test">
      <div class="goodclass">家务</div>
      <ul>
        <li><img src="./onegood.jpg" alt=""></li>
        <li><img src="./onegood.jpg" alt=""></li>
        <li><img src="./onegood.jpg" alt=""></li>
        <li><img src="./onegood.jpg" alt=""></li>
        <li><img src="./onegood.jpg" alt=""></li>
        <li><img src="./onegood.jpg" alt=""></li>
        <li><img src="./onegood.jpg" alt=""></li>
        <li><img src="./onegood.jpg" alt=""></li>
        <li><img src="./onegood.jpg" alt=""></li>
      </ul>
    </div>
  </div>
</template>

<script>
    import commonheader from '../commonheader/commonheader.vue'
    import {Search} from 'mint-ui'
    export default{
        created(){
          this.con='全部产品'
        },
        components: {
            commonheader,
            'mt-search': Search
        }
    }
</script>

<style lang='stylus' rel='stylesheet/stylus'>
  .goodsearch
    position relative
    .searchinput
      width: 100%;
      height: 3rem;
      background-color: #fff;
      background-image: url('./search.png');
      background-repeat: no-repeat;
      background-position: 38% .5rem;
      background-size: auto 70%;
      border-radius: 6px;
      text-align: center;
      font-size: 1.6em;
      color: #1f5350;
      font-family: Microsoft YaHei;
      padding-left: 3rem;
      position: absolute;
      left: 0;
      top: 0;
      z-index: 5;
      border none
  .test
    .goodclass
      height 10rem
      font-size 30px
      color red
    ul
      li
        display inline-block
        background-color lightskyblue
</style>
<style type="text/css" scoped>
  body{
    background-color: #fa131f;
  }
</style>

