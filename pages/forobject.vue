<template>
  <ul id="v-for-object" class="demo">
    <li v-for="(value, name, index) in object" v-bind:key="value">
      {{ index }}.{{ name }} : {{ value }}
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      object: {
        title: 'How to do lists in Vue',
        author: 'Jane Doe',
        publishedAt: '2016-04-10',
      },
    }
  },
}
</script>

<style scoped></style>
