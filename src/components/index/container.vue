<template>
  <div class="container">
    <channel-tag/>
    <row-a/>
  </div>
</template>
<script>
import RowA from '../index/rowa.vue'
import ChannelTag from '../index/channelTag.vue'
export default {
  components: { RowA, ChannelTag }
}
</script>