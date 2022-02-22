<template>
  <div id="app">
    <mySlider></mySlider>
  </div>
</template>

<script>
import mySlider from './components/mySlider.vue'

export default {
  name: 'App',
  components: {
    mySlider,
  }
}
</script>

<style>
  @import "./assets/style/general.scss";
</style>
