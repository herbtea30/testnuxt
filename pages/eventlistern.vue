<template>
  <div id="example-1">
    <button @click="counter += 1">Add 1</button>
    <p>위 버튼을 클릭한 횟수는 {{ counter }} 번 입니다.</p>
  </div>
</template>

<script>
export default {
  name: 'Eventlistern',
  data() {
    return {
      counter: 0,
    }
  },
}
</script>

<style scoped></style>
