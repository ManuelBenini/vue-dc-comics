<template>
<div class="categories">

  <div class="container mb-container">

    <ul class="d-flex">

      <li v-for="(category, index) in categories" :key="`image(${index})`">
        <div class="image">
          <img :class="{'shop-locator' : category.class != null}" :src="category.path" alt="">
        </div>
        <div class="category-name">
          <a href="#">{{category.name}}</a> 
        </div>
      </li>

    </ul>

  </div>

</div>
  
</template>

<script>
export default {
  name: 'CategoriesComp',
  data(){
    return{
      categories: [
        {
          name: 'DIGITAL COMICS',
          path: require('../assets/img/buy-comics-digital-comics.png'),
          class: null
        },
        {
          name: 'DC MERCHANDISE',
          path: require('../assets/img/buy-comics-merchandise.png'),
          class: null
        },
        {
          name: 'SUBSCRIPTION',
          path: require('../assets/img/buy-comics-subscriptions.png'),
          class: null
        },
        {
          name: 'COMIC SHOP LOCATOR',
          path: require('../assets/img/buy-comics-shop-locator.png'),
          class: 'shop-locator'
        },
        {
          name: 'DC POWER VISA',
          path: require('../assets/img/buy-dc-power-visa.svg'),
          class: null
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables';
@import '../assets/style/mixin';

.categories{
  background-color: $primary-color;
  
  .mb-container{
    min-height: 170px;
    @include align-center();
  }

  li{
    margin-right: 40px;
    padding-right: 20px;
    @include align-center();
    .image{
      width: 50px;
      margin-right: 10px;
      img{
        width: 100%;
      }
      .shop-locator{
        width: 70%;
      }
    }
  }
  
}

</style>