<template>
  <button>{{ label }}</button>
</template>

<script>
export default {
  name: 'TButton',
  props: {
    label: {
      type: String,
      required: true
    },
    color: {
      type: String,
      default: 'red'
    }
  }
}
</script>

<style lang="scss" scoped>
  $bg: red;
  button {
    background: $bg;
  }



</style>