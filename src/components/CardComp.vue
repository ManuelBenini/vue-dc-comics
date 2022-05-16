<template>
  <div class="d-flex flex-wrap">
      <div class="mb-card d-flex flex-column" v-for="(serie, index) in comics" :key="`serie${index}`">
        <div class="mb-series-thumbnail">
          <img :src="serie.thumb" alt="">
        </div>

        <h6>{{serie.series.toUpperCase()}}</h6>
      </div>
  </div>
</template>

<script>
export default {
    name: 'CardComp',
    props:{
        comics: Array
    }
}

</script>

<style lang="scss" scoped>
.mb-card{
    color: white;
    margin: 10px 0;
    width: calc(100% / 6);
    min-height: 250px;
    padding-right: 10px;
    padding-left: 20px;
    .mb-series-thumbnail{
        height: 193px;
        overflow: hidden;
        img{
        width: 100%;
        }
    }
    h6{
        margin: 10px 0;
    }
}
</style>