<template>
  <ul id="example-1">
    <li v-for="item in items" v-bind:key="item">
      {{ item.message }}
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      items: [{ message: 'Foo' }, { message: 'Bar' }, { message: 'Seojun' }],
    }
  },
}
</script>

<style scoped></style>
