<template>
  <h1 v-if="awesome">Vue is aweswome!</h1>
  <h1 v-else>Oh no 😊</h1>
</template>
<script>
export default {
  data() {
    return {
      awesome: true,
    }
  },
}
</script>

<style></style>
