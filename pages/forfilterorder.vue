<template>
  <ul>
    <li v-for="n in even(numbers)" :key="n">{{ n }}</li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      numbers: [1, 2, 3, 4, 5],
    }
  },
  methods: {
    even() {
      return this.numbers.filter(function (number) {
        return number % 2 === 0
      })
    },
  },
}
</script>

<style scoped></style>
