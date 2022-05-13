<template>
<div class="categories">

  <div class="container mb-container">

    <ul class="d-flex">

      <li>
        <div class="image">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
        </div>
        <div class="category-name">
          <a href="#">Digital Comics</a> 
        </div>
      </li>

      <li>
        <div class="image">
          <img src="../assets/img/buy-comics-merchandise.png" alt="">
        </div>
        <div class="category-name">
          <a href="#">DC MERCHANDISE</a> 
        </div>
      </li>

      <li>
        <div class="image">
          <img src="../assets/img/buy-comics-subscriptions.png" alt="">
        </div>
        <div class="category-name">
          <a href="#">SUBSCRIPTION</a> 
        </div>
      </li>

      <li>
        <div class="image">
          <img class="shop-locator" src="../assets/img/buy-comics-shop-locator.png" alt="">
        </div>
        <div class="category-name">
          <a href="#">COMIC SHOP LOCATOR</a> 
        </div>
      </li>

      <li>
        <div class="image">
          <img src="../assets/img/buy-dc-power-visa.svg" alt="">
        </div>
        <div class="category-name">
          <a href="#">DC POWER VISA</a> 
        </div>
      </li>

    </ul>

  </div>

</div>
  
</template>

<script>
export default {
  name: 'CategoriesComp',
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