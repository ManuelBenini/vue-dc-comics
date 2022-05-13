<template> 

  <div>

      <HeaderComp/>
      <MainComp/>
      <ShopCategories/>
      <FooterComp/>
      <FooterBottom/>

  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import MainComp from './components/MainComp.vue'
import ShopCategories from './components/ShopCategories.vue'
import FooterComp from './components/FooterComp.vue'
import FooterBottom from './components/FooterBottom.vue'

export default {
  name: 'App',
  components: {
    MainComp,
    HeaderComp,
    ShopCategories,
    FooterComp,
    FooterBottom
}
}
</script>

<style lang="scss">

@import './assets/style/variables';
@import './assets/style/globals';
@import './assets/style/utilities';

</style>
