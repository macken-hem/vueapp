<template>
  <div>
    <p>カウントアップ({{ number }})</p>
    <button v-on:click="increment">+1</button>
    <a v-bind:href ="url">Github</a>
    <p v-on:mousemove="mousePosition">10000000000</p>
    <p>X{{x}},Y{{y}}</p>
    <h2>aaaa</h2>
    <img v-show="uploadedImage" :src="uploadedImage"/>
    <input type="file" v-on:change="onFileChange">
  </div>
</template>

<script>
export default {
  data() {
    return {
      number: 0,
      url : "https://github.com/macken-hem/vueapp",
      x: 0,
      y: 0,
      uploadedImage: ''
    };
  },
  methods: {
    increment() {
      this.number += 1;
    },
    mousePosition(event){
      this.x = event.clientX
      this.y = event.clientY
    },
    onFileChange(e) {
      let files = e.target.files || e.dataTransfer.files;
      this.createImage(files[0]);
    },
    createImage(file) {
      let reader = new FileReader()
      reader.onload = (e) => {
        this.uploadedImage = e.target.result;
      };
      reader.readAsDataURL(file);
    }
  }
};
</script>

<style scoped>
div {
  width: 100%;
  height: 100%;
  background-color: blanchedalmond;
}
</style>