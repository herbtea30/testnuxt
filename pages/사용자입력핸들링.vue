<template>
  <div id="app-5">
    <p>{{ message }}</p>
    <button @click="reverseMessage">메세지 뒤집기</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: '안녕하세요. Vue.js!',
    }
  },
  methods: {
    reverseMessage() {
      this.message = this.message.split('').reverse().join('')
    },
  },
}
</script>

<style></style>
