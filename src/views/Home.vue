<template>
  <div class="home">
    <top-view />
    <sales-view />
    <bottom-view />
    <map-view />
  </div>
</template>

<script>
// @ is an alias to /src
import TopView from '../components/topView'
import SalesView from '../components/salesView'
import BottomView from '../components/bottomView'
import MapView from '../components/mapView'
export default {
  name: 'Home',
  components: {
    TopView,
    SalesView,
    BottomView,
    MapView
  }
}
</script>

<style scoped>
  .home {
    width: 100%;
    height: 100%;
    padding: 20px;
    background: #eeeeee;
    box-sizing: border-box;
  }
</style>
