<template>
    <x-header :left-options="{showBack: false}">发表评价<img slot="left" src="../assets/back.png"></x-header>
</template>

<script>
import $ from 'jquery'
import { XHeader } from 'vux'
export default {
  components: {
    XHeader
  },
  data () {
    return {
    }
  },
  mounted () {
    $('.vux-header').css({
      'background-color': 'white'
    }),
    $('.vux-header-title').css({
      'color': 'black',
      'font-size':'18px'
    })
  }
}
</script>
<style>
  img{
    width: 20px;
  }
</style>
jquery