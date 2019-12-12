<template>
  <div>
    <p>いいね({{ number }})</p>
    <button @click="increment">+1</button>
    <a v-bind:href ="url">Github</a>
  </div>
</template>

<script>
export default {
  data() {
    return {
      number: 0,
      url : "https://github.com/macken-hem/vueapp"
    };
  },
  methods: {
    increment() {
      this.number += 1;
    }
  }
};
</script>
