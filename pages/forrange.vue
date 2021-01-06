<template>
  <div>
    <li v-for="n in 10" :key="n">{{ n }}</li>
  </div>
</template>

<script>
export default {
  name: 'Forrange',
}
</script>

<style scoped></style>
