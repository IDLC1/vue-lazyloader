<template>
  <div id="app">
    <div v-for="img in imgs"  :key="img">
      <!-- <img data-src="./assets/logo.png" v-lazy="img"> -->
      <div v-lazy-container="{ selector: 'img', error: './assets/logo.pg', loading: 'xxx.jpg' }">
        <img :data-src="img" lazy="loading">
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'App',
  data() {
    return {
      imgs: [
            "http://ww4.sinaimg.cn/large/006y8mN6gw1fa5obmqrmvj305k05k3yh.jpg",
            "http://ww1.sinaimg.cn/large/006y8mN6gw1fa7kaed2hpj30sg0l9q54.jpg",
            "http://file02.16sucai.com/d/file/2014/0829/372edfeb74c3119b666237bd4af92be5.jpg",
            "http://file02.16sucai.com/d/file/2014/0704/e53c868ee9e8e7b28c424b56afe2066d.jpg",
            "http://g.hiphotos.baidu.com/zhidao/pic/item/ac4bd11373f08202b4a9a53a4bfbfbedab641bff.jpg",
            "http://b2-q.mafengwo.net/s5/M00/91/06/wKgB3FH_RVuATULaAAH7UzpKp6043.jpeg",
            "http://e.hiphotos.baidu.com/zhidao/pic/item/0bd162d9f2d3572c75676abf8a13632763d0c3c8.jpg",
            "http://image.uisdc.com/wp-content/uploads/2014/02/ea4b4111a08b342a40d11d89a349b20d_m.jpg",
            "http://file02.16sucai.com/d/file/2014/0829/b871e1addf5f8e96f3b390ece2b2da0d.jpg",
            "http://file02.16sucai.com/d/file/2014/0920/9865f4ed66ec1829fed3fd626689c448.jpg"
          ]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>
