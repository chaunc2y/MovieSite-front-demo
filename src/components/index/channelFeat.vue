<template>
  <div class="channel">
    <channel-title/>
    <row-b/>
    <Banner/>
  </div>
</template>
<script>
import RowB from '../index/rowb.vue'
import Banner from '../index/banner.vue'
import ChannelTitle from '../index/titleFea.vue'
export default {
  components: { RowB, Banner, ChannelTitle }
}
</script>
