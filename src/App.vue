<template>
  <div id="app">
    <!-- <poster></poster>
    <router-view></router-view> -->

    <!-- <template >
      <poster></poster>
    </template> -->
    <!-- <template >
      <router-view />
    </template> -->

    <router-view></router-view>
    
<!-- <div @click="sss">===================</div> -->
  </div>
</template>


<script setup lang="ts">
import { onLaunch, onShow, onHide } from "@dcloudio/uni-app";
onLaunch(() => {
  console.log("App Launch", uni);

  uni.showToast({
      title: '测试弹窗',
      icon: 'error',
      duration: 5000,
    });

});
onShow(() => {
  console.log("App Show");
});
onHide(() => {
  console.log("App Hide");
});
</script>
<style></style>
