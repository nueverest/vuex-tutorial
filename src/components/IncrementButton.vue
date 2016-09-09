<template>
  <div>
    <button @click.prevent="activate">+1</button>
  </div>
</template>

<script>
  import store from '../vuex-store'

  export default {
    methods: {
      activate () {
        store.dispatch('INCREMENT')
        console.log('+1 Pressed')
      }
    }
  }
</script>


<!--<style scoped></style>-->
