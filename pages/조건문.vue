<template>
  <div id="app3">
    <p v-if="seen">이제 나를 볼 수 있어요</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      seen: true,
    }
  },
}
</script>
