<template>
  <div class="goodsinfo_wrap">
      <div class='goodsinfo'>
          <div class='goods_img'>
              <img src="../assets/computer.jpg" alt="">
          </div>
          <div class='goods_text'>
              <p>3件装|MEDIHEAL 小米笔记本 4核 128g固态硬盘 14.6英寸屏幕 你值得拥有</p>
              <p>颜色： 蓝 尺码： XL</p>
          </div>
      </div>
      <div class='goodsstar'>
          <div class='goodsstar_left'>
              <p>商品描述</p>
          </div>
          <div class='goodsstar_middle'>
              <rater v-model="data42" active-color="#04BE02" :font-size="15" disabled></rater>
          </div>
          <div class='goodsstar_right'>
              <p>非常好</p>
          </div>
      </div>
  </div>
</template>

<script>

import { Rater } from 'vux'
export default {
  components: {
    Rater
  },
  data () {
    return {
        data42: 3.5
    }
  }
}
</script>
<style>
  .goodsinfo_wrap{
      background-color: white;
  }
  .goodsinfo{
      display: flex;
      padding-top:10px;
      padding-bottom: 5px;
      border-top: 1px solid lightgrey;
  }
  .goodsinfo .goods_img{
      flex: 1;
      margin-left: 10px;
  }
  .goodsinfo .goods_text{
      flex: 4;
      margin-left: 15px;
      margin-right: 15px;
  }
  .goods_img img{
      width: 100%;
  }
  .goodsstar{   
      display: flex;
      /* height: 50px; */
      padding-top: 10px;
      padding-bottom: 10px;
      margin-left: 10px;
      margin-right: 10px;
      /* text-align: center; */
      border-top: 1px solid lightgray;
  }
  .goodsstar .goodsstar_left{
      flex: 1;
      font-size: 13px;
      /* background-color: brown; */
      margin-top: 3px;
  }
  .goodsstar .goodsstar_middle{
      flex: 1;
      /* background-color:lightgrey; */
  }
  .goodsstar .goodsstar_right{
      flex: 1;
      /* margin-right: 0px; */
      text-align: right;
      /* background-color: lightgreen; */
      font-size: 10px;
      color:grey;
      margin-top: 3px;
  }
  .goods_text>p:nth-child(1){
      font-size: 13px;
      overflow : hidden;
      text-overflow: ellipsis;
      display: -webkit-box;
      -webkit-line-clamp: 2;
      -webkit-box-orient: vertical;
  }
  .goods_text>p:nth-child(2){
      overflow : hidden;
      text-overflow: ellipsis;
      display: -webkit-box;
      -webkit-line-clamp: 2;
      -webkit-box-orient: vertical;
      font-size: 12px;
      color:orange;
  }
</style>
