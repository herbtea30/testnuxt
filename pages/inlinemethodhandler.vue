<template>
  <div id="example-3">
    <button @click="say('hi')">Say hi</button>
    <button @click="say('what')">Say what</button>
    <button @click="warn('Form cannot be submitted yet.', $event)">
      Submit
    </button>
  </div>
</template>

<script>
export default {
  name: 'Inlinemethodhandler',
  methods: {
    say(message) {
      alert(message)
    },
    warn(message, event) {
      if (event) event.preventDefault()
      alert(message)
    },
  },
}
</script>

<style scoped></style>
