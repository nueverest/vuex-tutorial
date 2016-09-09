<template>
  Count is {{ count }}
</template>

<script>
  import store from '../vuex-store'

  export default {
    computed: {
      count () {
        console.log(store.state.counter)
        return store.state.counter
      }
    }
  }
</script>

<style scoped></style>
