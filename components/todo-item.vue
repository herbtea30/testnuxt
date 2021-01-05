<template>
  <li>{{ todo.text }}</li>
</template>

<script>
export default {
  props: {
    todo: {
      type: Function,
      default: () => {},
    },
  },
}
</script>

<style></style>
