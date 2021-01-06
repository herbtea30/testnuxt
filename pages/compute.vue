<template>
  <div id="example">
    <p>원본 메세지: "{{ message }}"</p>
    <p>역순으로 표시한 메세지: "{{ reverseMessage }}"</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: '안녕하세요',
    }
  },
  computed: {
    reverseMessage() {
      return this.message.split('').reverse().join('')
    },
  },
}
</script>

<style></style>
