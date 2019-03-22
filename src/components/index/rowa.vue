<template>
  <div class="split">
    <div class="row">
      <left-side/>
      <right-side/>
    </div>
  </div>
</template>
<script>
import LeftSide from '../index/leftside.vue'
import RightSide from '../index/rightside.vue'
export default {
  components: { LeftSide, RightSide }
}
</script>
