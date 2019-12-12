<template>
<header>
  <div class = "head-ber">
    <h3>TOP</h3>
    <h3>ABOUT</h3>
    <h3>EXPERIENCE</h3>
    <h3>PORTFOLIO</h3>
    <h3>PICTURE</h3>
  </div>
</header>
</template>

<script>
export default {
  data (){
    return {
    profile: "プロフィール"
    }
  }
}
</script>

<style scoped>
div {
  display: flex;
  justify-content: space-between;
}

header {
  height: 100%;
  width: 100%;
  background-color: rgba(48, 187, 241, 0.479);
  box-shadow:0px 4px rgba(9, 110, 224, 0.082);
}

.head-ber {
  width: 80%;
  margin: 0 auto;
}

</style>