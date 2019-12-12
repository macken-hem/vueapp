<template>
  <div>
    <header>aaaaaaa</header>
    <LikeHeader></LikeHeader>
    <LikeNumber></LikeNumber>
  </div>
</template>

<script>
import 'normalize.css'
import LikeHeader from "./components/LikeHeader.vue"

export default {
  components: {
    LikeHeader
  }
};
</script>

<style scoped>
header {
  height: 80px;
  width: 100%;
  background-color: rgba(0, 119, 255, 0.479);
}
div {
  border: 1px solid blue;
}
</style>