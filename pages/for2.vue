<template>
  <ul id="example-2">
    <li v-for="(item, index) in items" v-bind:key="index">
      {{ parentMessage }} - {{ index }} - {{ item.message }}
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      parentMessage: 'Parent',
      items: [{ message: 'Foo' }, { message: 'Bar' }],
    }
  },
}
</script>

<style scoped></style>
