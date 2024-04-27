<template>
  <ul>
    <li>{{ listItems[0] }}</li>
    <li>{{ listItems[1] }}</li>
    <li>{{ listItems[2] }}</li>
  </ul>
</template>

<script>

export default {
  name: 'TList',
  props: {
    listItems: {
      type: Array,
      required: true
    }
  }
}

</script>