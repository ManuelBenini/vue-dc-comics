<template>

  <main>

    <JumbotronComp/>

    <div class="container mb-container">

      <div class="mb-current-series">CURRENT SERIES</div>

      <CardComp :comics='comics'/>

      <div class="moreBtn">
        <button class="mb-load-more">LOAD MORE</button>
      </div>

    </div>
    
  </main>

</template>

<script>
  import comicsJson from '../assets/data/comics.json'
  import CardComp from './CardComp.vue'
  import JumbotronComp from './JumbotronComp.vue';

  export default {
    name: "MainComp",
    data() {
        return {
            comics: comicsJson
        };
    },
    components: { CardComp, JumbotronComp }
  }
</script>

<style lang="scss" scoped>

  @import "../assets/style/mixin";
  @import "../assets/style/variables";

  main{
    background-color: #1c1c1c;
    .mb-container{
      position: relative;
      padding: 35px 0 20px 0;
      .mb-current-series{
        position: absolute;
        top: -20px;
        left: 0px;
        border: none;
        background-color: $primary-color;
        color: white;
        padding: 5px 15px;
        font-weight: bold;
        font-size: 17px;
      }
      .moreBtn{
        text-align: center;
        .mb-load-more{
          border: none;
          padding: 5px 50px;
          background-color: $primary-color;
          color: white;
          margin-top: 30px;
        }
      }
      
    }
  }

</style>