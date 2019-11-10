<template>
  <section class="container">
    <weather
      api-key="///826a2861d1a67df803840425d4bbb6c4／／／"
      title="Weather for GuangZhou "
      units="uk"
      :latitude="lat"
      :longitude="long"
      language="en"
    ></weather>
  <baidu-map class="map">
  </baidu-map>
  </section>
</template>
<script>

import Weather from 'vue-weather-widget'
import Vue from 'vue'
import BaiduMap from 'vue-baidu-map'
export default {
  name: 'app',
  components: {
    Weather
  },
  data: () => ({
    lat: '23.11337',
    long: '113.25523'
  })
}
Vue.use(BaiduMap, {
  ak: 'ngwsmyC1ss4K2kX0cNTpVwpI4gqQOVP1'
})
</script>

<style>
.container {
  height: 100px;
  width: 920px;
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 4px;
}
</style>
