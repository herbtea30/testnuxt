<template>
  <div id="demo">
    {{ fullName }}
  </div>
</template>

<script>
export default {
  data() {
    return {
      firstName: 'Foo',
      lastName: 'Bar',
      // fullName: 'Foo Bar',
    }
  },
  computed: {
    fullName: {
      get() {
        return this.firstName + ' ' + this.lastName
      },
      set(newValue) {
        const names = newValue.split(' ')
        this.firstName = names[0]
        this.lastName = names[names.length - 1]
      },
    },
  },
  //   watch: {
  //     firstName(val) {
  //       this.fullName = val + ' ' + this.lastName
  //     },
  //     lastName(val) {
  //       this.fullName = this.firstName + ' ' + val
  //     },
  //   },
}
</script>

<style></style>
