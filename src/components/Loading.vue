<template>
  <div id="fullOverlay">
    <div class="fullview">
      <div class="loading-spacer"></div>
      <vue-loading
        type="cylon"
        color="#42b883"
        :size="{ width: '100px', height: '100px' }"
        >
      </vue-loading>
    </div>
  </div>
</template>

<script>
import { VueLoading } from 'vue-loading-template'

export default {
  name: 'loading',
  components: {
    VueLoading,
  },

}
</script>

<style>
.fullview {
  width: 100%;
  height: 100%;
   background: rgba(100, 100, 100, .8);
  position: fixed;
  top: 70px;
  left: 0;
}
.loading-spacer {
  height: 30%;
}


</style>