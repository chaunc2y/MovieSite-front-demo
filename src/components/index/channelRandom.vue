<template>
  <div class="box">
    <channel-title/>
    <box-content/>
  </div>
</template>
<script>
import ChannelTitle from '../index/titleRan.vue'
import BoxContent from '../index/boxcontentRan.vue'
export default {
  components: {
    ChannelTitle,
    BoxContent
  }
}
</script>

