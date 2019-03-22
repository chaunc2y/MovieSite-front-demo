<template>
  <div id="main-content-b" class="col-md-8 col-sm-12 col-xs-12">
    <channel-feat/>
    <channel-random/>
    <channel-hot/>
    <channel-new/>
  </div>
</template>
<script>
import ChannelFeat from '../index/channelFeat.vue'
import ChannelRandom from '../index/channelRandom.vue'
import ChannelHot from '../index/channelHot.vue'
import ChannelNew from '../index/channelNew.vue'
export default {
  components: { ChannelFeat, ChannelRandom, ChannelHot, ChannelNew }
}
</script>
