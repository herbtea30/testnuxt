<template>
  <div id="app-6">
    <p>{{ message }}</p>
    <input v-model="message" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: '안녕하세요 vue.js!',
    }
  },
}
</script>

<style></style>
