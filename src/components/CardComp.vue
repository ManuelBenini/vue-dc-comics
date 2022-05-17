<template>

  <div class="mb-card">
    <div class="logo">
      <img :src="serieData.thumb" alt="serieThumbnail">
    </div>

    <h6 class="my-3">{{serieData.series.toUpperCase()}}</h6>
  </div>
  
</template>

<script>
export default {
  name: 'CardComp',
  props:{
    serieData: Object
  }
}
</script>

<style lang="scss" scoped>

  .mb-card{
    width: calc(100% / 6);
    margin-top: 15px;
    .logo{
      height: 192px;
      overflow: hidden;
    }
    h6{
      color: white;
    }
  }

</style>