<template>
  <input
      @change="handleChange"
  >
</template>

<script>
  export default {
    name: 'ElInput',
    data () {
      return {}
    },
    methods: {
      handleChange (event) {
        this.$emit('change', event.target.value)
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
