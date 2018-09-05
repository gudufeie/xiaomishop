<template>
  <div class="page_wrap">
    <div class="title">
      <tou></tou>
    </div>
    <div class="content">
      <goodsinfo></goodsinfo>
    </div>
    <div class="bottom">
      <goodsmiaoshu></goodsmiaoshu>
    </div>
    <div class="subbtn">
      <subbtn></subbtn>
    </div>
  </div>
</template>

<script>

import tou from './tou.vue'
import goodsinfo from './goodsinfo.vue'
import subbtn from './subbtn.vue'
import goodsmiaoshu from './goodsmiaoshu.vue'
export default {
  components: {
    tou,
    goodsinfo,
    subbtn,
    goodsmiaoshu
  },
  data () {
    return {

    }
  }
}
</script>
<style>
  .page_wrap{
    height: 800px;
    background-color: rgb(235, 231, 231);
  }
  .bottom{
    /* height: 150px; */
    /* background-color:orange; */
  }
  .subbtn{
    margin-top: 20px;
  }
</style>
