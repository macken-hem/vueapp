<template>
  <div>
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
div {
  border: 1px solid blue;
}
</style>