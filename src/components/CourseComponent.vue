<template>

</template>

<script>
import { ref } from 'vue'

export default {
setup () {
  return {
    expanded: ref(false),
    lorem: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.'
  }
}
}
</script>

<style lang="sass" scoped>
.my-card
width: 10%
max-width: 350px
</style>
