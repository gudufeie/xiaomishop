<template>
  <div class="miaoshu_wrap">
    <div class="miaoshu_top">
        <p>商品描述</p>
    </div>
    <div calss="miaoshu_middle">
      <x-textarea :height="130"></x-textarea>
    </div>
    <div class="miaoshu_bottom" @click="select_tu">
        <div class="picture">
          <img src="../assets/xiangji.png" alt="">
          <p>添加图片</p>
        </div>
    </div>
  </div>
</template>

<script>

import $ from 'jquery'
import { XTextarea } from 'vux'
export default {
  components: {
      XTextarea
  },
  data () {
    return {

    }
  },
  methods: {
      select_tu() {
        console.log("***********************************")
      }
  },
  mounted (){
    $('.weui-textarea').css({
      'background-color':'lightgrey'
  })
  }
}
</script>
<style>
    .miaoshu_wrap{
        margin-top: 5px;
        background-color: white;
        padding-top: 10px;
    }
    .miaoshu_top{
        margin-left: 10px;
        font-size: 13px;
    }
    .miaoshu_middle{
        font-size: 13px;
    }
    .miaoshu_bottom{
        margin-left: 12px;
        font-size: 10px;
        padding-bottom: 10px;
    }
    .miaoshu_bottom .picture{
        /* display: inline-block; */
        width:50px;
        padding: 8px;
        border: 1px dotted lightgray;
    }
    .miaoshu_bottom .picture img{
        width: 50%;
        display: block;
        margin-left: 13px;
    }
    .miaoshu_bottom .picture p{
        font-size: 10px;
        display: block;
    }
</style>
