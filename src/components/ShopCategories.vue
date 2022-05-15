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
import digitalComicsLogo from "../assets/img/buy-comics-digital-comics.png";
import dcMerchandiseLogo from "../assets/img/buy-comics-merchandise.png";
import subscriptionLogo from "../assets/img/buy-comics-subscriptions.png";
import comicShopLocatorLogo from "../assets/img/buy-comics-shop-locator.png";
import dcPowerVisaLogo from "../assets/img/buy-dc-power-visa.svg";

export default {
  name: 'CategoriesComp',
  data(){
    return{
      categories: [
        {
          name: 'DIGITAL COMICS',
          path: digitalComicsLogo,
          class: null
        },
        {
          name: 'DC MERCHANDISE',
          path: dcMerchandiseLogo,
          class: null
        },
        {
          name: 'SUBSCRIPTION',
          path: subscriptionLogo,
          class: null
        },
        {
          name: 'COMIC SHOP LOCATOR',
          path: comicShopLocatorLogo,
          class: 'shop-locator'
        },
        {
          name: 'DC POWER VISA',
          path: dcPowerVisaLogo,
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