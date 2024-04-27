<template>
  <div>
    <label :for="inputId">{{ label }}</label>
    <input :id="inputId" :type="inputType" :disabled="isDisabled" />
  </div>
</template>

<script>

export default {
  name: 'TInput',
  props: {
    inputId: {
      required: true,
      type: String
    },
    label: {
      type: String,
      default: ''
    },
    inputType: {
      type: String,
      default: 'text'
    },
    isDisabled: {
      type: Boolean,
      default: false,
    }
  }
}

</script>

<style scoped>
div {
  display: flex;
  flex-direction: column;
}
</style>