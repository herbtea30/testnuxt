<template>
  <button @click="greet">Greet</button>
</template>

<script>
export default {
  name: 'Methodeventhandle',
  data() {
    return {
      name: 'Vue.js',
    }
  },
  methods: {
    greet() {
      alert('Hello' + this.name + '!')
      if (event) {
        alert(event.target.tagName)
      }
    },
  },
}
</script>

<style scoped></style>
