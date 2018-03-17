<template>
  <div class="hello">
    <div class="banner-background" :style="homeBox"></div>
    <div class="first-page" :style="homeBox">
      <div class="title">{{msg}}</div>
      <div class="search-box">
        <div class="new-searching-unit">
          <input id="query" type="text" autocomplete="off" placeholder="find you like..." value="">
          <a class="go"></a></div>
        <div class="search-hint"></div>
      </div>
    </div>
    <Header></Header>
    <div class="img-container">
      <div v-for="index in 22" class="recommend-hidebox pl-right">
        <div class="recommend-box" :style="getRecommendBoxClass(index)"></div>
        <div class="recommend-infobox board recommend-box big">
          <div class="recommend-data board"></div>
          <h2><a>Picture name</a></h2>
          <p>Picture description</p>
          <div class="info-tra-left big"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import Header from './Header.vue'
  export default {
    name: 'hello',
    components: {
      Header
    },
    data () {
      return {
        msg: 'Welcome...',
        homeBox: {
          height: 'auto'
        },
        headerTop: false,
        testImg: 'static/img/demo-img.jpeg',
        imgCardData: [
          {
            name: 'Picture name',
            desc: 'Picture description',
            path: 'static/imglist/1114_1.jpeg'
          },
          {
            name: 'Picture name',
            desc: 'Picture description',
            path: 'static/imglist/1114_2.jpeg'
          },
          {
            name: 'Picture name',
            desc: 'Picture description',
            path: 'static/imglist/1114_3.jpeg'
          },
          {
            name: 'Picture name',
            desc: 'Picture description',
            path: 'static/imglist/1114_4.jpeg'
          },
          {
            name: 'Picture name',
            desc: 'Picture description',
            path: 'static/imglist/1114_5.jpeg'
          },
          {
            name: 'Picture name',
            desc: 'Picture description',
            path: 'static/imglist/1114_6.jpeg'
          },
          {
            name: 'Picture name',
            desc: 'Picture description',
            path: 'static/imglist/1114_7.jpeg'
          },
          {
            name: 'Picture name',
            desc: 'Picture description',
            path: 'static/imglist/1114_8.jpeg'
          },
          {
            name: 'Picture name',
            desc: 'Picture description',
            path: 'static/imglist/1114_9.jpeg'
          }
        ]
      }
    },
    created () {
      this.homeBox.height = window.innerHeight + 'px'
    },
    methods: {
      up () {
        console.log(window.scrollY)
        this.headerTop = true
      },
      getRecommendBoxClass (index) {
        let imgPath = 'static/imglist/1114_' + index + '.jpg'
        // this.imgCardData[index]['path']
        let obj = {
          background: 'url(' + imgPath + ')',
          'background-size': 'cover'
        }
        return obj
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
