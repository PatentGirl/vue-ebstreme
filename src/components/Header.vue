<template>
  <div id="header" class="hts" :class="{nologinIndex: headerTop}" style="left: 0px;" scroll-top="50" scroll-up="up()">
    <div class="wrapper wrapper-996">
      <div class="menu-bar">
        <div class="left-part">
          <a id="logo" href="/"></a>
          <a class="header-item active"><router-link :to="{name: 'Hello'}">Home</router-link></a>
          <a class="header-item "><router-link :to="{name: 'Profile'}">Profile</router-link></a>
          <a class="header-item "><router-link :to="{name: 'Bunch'}">Bunch</router-link></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: '',
    data () {
      return {}
    },
    methods: {}
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
