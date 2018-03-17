<template>
  <div class="bunch" :style="bunchBox">
    <Header></Header>
    <div class="bunch-left">
      <div class="bunch-list">
        <ul>
          <li class="list-c on"></li>
          <li class="list-c"></li>
          <li class="list-c"></li>
          <li class="list-c"></li>
          <li class="list-c"></li>
          <li class="list-c"></li>
        </ul>
        <!--<div class="bunch-icon-footer">-->
          <!--<router-link :to="{name: 'Hello'}"><span class="fx-return"><img src="../assets/icon/icon-return.png"/></span></router-link>-->
          <!--<span><img src="../assets/icon/icon-reference.png"/></span>-->
        <!--</div>-->
        <div class="bunch-lest-footer">
          <span>eBstreme</span>
        </div>
      </div>
      <div class="bunch-content">
        <h1>BUNCH</h1>
        <div>
          <h4>WHAT WE DO</h4>
          <p>eBstreme Limited introduces its organic or natural fresh fruit juice blend, ‘BUNCH’. The company offers this product to its cherished customers. Since we aim to serve our customers with fresh products, our juices are not mixed and stored but are produced at their request. </p>
        </div>
        <div>
          <p>What makes ‘BUNCH’ unique is the fact that patrons get to choose from a wide range of fruit mixes. Thus, at eBstreme we make raw organic fruit juice mix readily available and affordable to everyone with the aim of helping to promote a healthy lifestyle. </p>
          <p>We also take orders for office lunch, parties, corporate events (including meetings), weddings, conferences and many more. </p>
        </div>
        <div class="content-box">
          <h4>OUR TEAM</h4>
          <p class="info">
            <span>Ebenezer Osei Asante – Managing Director</span>
            <span>Benjamin Osei – Administration / Marketing Manager</span>
            <span>Eunice Mensah  – Finance Manager</span>
            <span>Abraham Joana Osei – Operations Manager</span>
            <span>Cynthia Adjei – Purchase / Health & Quality Officer</span>
            <span>Dorcas Sasu-Antwi – Health & Quality Officer</span>
          </p>
        </div>
        <div class="content-box">
          <h4>OUR PRODUCT</h4>
          <p>‘Bunch’ is 100% natural or organic fruit juice blend. It is made from carefully selected fruits for the delight and satisfaction of our customers. ‘BUNCH’ juice mix contains NO artificial preservatives, color or added sugar.</p>
        </div>
      </div>
    </div>
    <div class="bunch-right">
      <div class="mix"><span>MIX FRUIT JUICE MIX</span></div>
      <div class="bunch-frout"><img src="../assets/img/bunch-fruit.png"></div>
      <div class="info">
        <span>OUR CONTACT</span>
        <span>Benjamin Osei</span>
        <span>eBstreme Limited</span>
        <span>Post Office Box AN10246, Accra North.</span>
        <span>Tel : 00233 24 211 2925 /</span>
        <span> 00233 24 323 1616 / 00233 20 887 6123 </span>
        <span>Email: bunchjuice@gmail.com</span>
      </div>
    </div>
  </div>
</template>

<script>
  import Header from './Header.vue'
  export default {
    name: 'bunch',
    components: {
      Header
    },
    data () {
      return {
        bunchBox: {
          height: 'auto'
        }
      }
    },
    created () {
      this.bunchBox.height = window.innerHeight + 'px'
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.bunch {
  background-color: #37AA11;
}
</style>
