<template>
  <div id="app">
    <tiny-slider :mouse-drag="true" :loop="false" items="1" gutter="0" axis="vertical" :nav="false" :controls="false">
      <BannerComponent></BannerComponent>
      <AboutComponent></AboutComponent>
    </tiny-slider>
  </div>
</template>

<style lang="scss">

</style>
<script>
import BannerComponent from '@/components/BannerComponent'
import VueTinySlider from 'vue-tiny-slider'
import './lib/tiny-slider.css'
import AboutComponent from '@/components/AboutComponent'

export default {
  components: {
    AboutComponent,
    BannerComponent,
    'tiny-slider': VueTinySlider
  }
}
</script>
<style lang="scss">
  body{
    font-family: 'Poppins', sans-serif;
  }
  :root{
    --bg-opacity: 1;
  }
</style>
