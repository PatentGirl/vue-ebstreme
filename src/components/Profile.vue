<template>
  <div class="body bg-c" :style="profileBox">
    <Header></Header>
    <div class="g-back">
      <div class="p-content">
        <h1 class="p-name">Profile</h1>
        <div class="p-text">
          <img src="../assets/icon/icon-me.png"/>
          <p class="profile-p">
            The eBstreme group of companies is an establish
            leadership and pioneer in  various industries such as,MEDIA
            (eBstreme motion and eBstreme graphics),Food and beverage
            (BUNCH) , conceptual design,with the aim of providing high
            quality of product and services at a very competitive prices.
          </p>
          <br>
          <p class="profile-p">
            Our companys HQ is based in Accra Ghana W/A,with 12 years of
            providing services to our client in Canada,china,Taiwan(welsin),
            Ghana (denifas Ent.)Congo and Uganda
          </p>
        </div>
      </div>
      <!--<div class="p-footer">-->
        <!--<router-link :to="{name: 'Hello'}"><span class="fx-return"><img src="../assets/icon/icon-return.png"/></span></router-link>-->
        <!--<span><img src="../assets/icon/icon-reference.png"/></span>-->
        <!--&lt;!&ndash;<span class="p-signature">eBstreme</span>&ndash;&gt;-->
      <!--</div>-->
    </div>
    <span class="p-signature">eBstreme</span>
  </div>
</template>

<script>
  import Header from './Header.vue'
  export default {
    name: 'profile',
    components: {
      Header
    },
    data () {
      return {
        profileBox: {
          height: 'auto'
        }
      }
    },
    created () {
      this.profileBox.height = window.innerHeight + 'px'
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


</style>
