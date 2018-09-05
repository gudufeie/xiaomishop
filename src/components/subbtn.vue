<template>
  <div class="goodsmiaoshu_wrap">
    <button type="primary">提交评价</button>
  </div>
</template>

<script>
import { XButton } from 'vux'
export default {
  components: {
      XButton
  },
  data () {
    return {

    }
  },
  created (){

  }
}
</script>
<style>
    .goodsmiaoshu_wrap{
        padding-left: 25px;
        padding-right: 25px;
    }
    button{
        background: linear-gradient(red, rgb(134, 36, 36));;
        width:100%;
        height: 45px;
        border-radius: 99px;
        color: white;
        font-size: 16px;
    }
</style>
