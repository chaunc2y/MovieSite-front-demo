<template>
  <div class="box">
    <channel-title/>
    <box-content/>
    <div class="line"></div>
  </div>
</template>
<script>
import ChannelTitle from '../index/titleHot.vue'
import BoxContent from '../index/boxcontentHot.vue'
export default {
  components: {
    ChannelTitle,
    BoxContent
  }
}
</script>
<style>
.line {
  border-bottom: 1px solid #bbb;
  width: 100%;
  margin: 20px 0;
}
</style>


