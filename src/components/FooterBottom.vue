<template>
  <div class="footer-bottom">
      <div class="container mb-container">
          <div class="call-to-action">
              <a href="#">SIGN-UP NOW!</a>
          </div>

          <div class="socials">
              <div>
                  <span>FOLLOW US</span>
              </div>

              <div class="images">
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-twitter.png" alt="">
                <img src="../assets/img/footer-youtube.png" alt="">
                <img src="../assets/img/footer-pinterest.png" alt="">
                <img src="../assets/img/footer-periscope.png" alt="">  
              </div>
              
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'FooterSocials'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables';
@import '../assets/style/mixin';

.footer-bottom{
    background-color: #303030;
}
.mb-container{
    min-height: 83px;
    @include align-center();
    justify-content: space-between;

    .socials{
        display: flex;
        & div:first-child{
            margin-right: 20px;
        }
    }
    .call-to-action{
        padding: 5px;
        border: 2px solid $primary-color;
    }
    span{
        font-weight: bold;
        color: $primary-color;
    }
    img{
        width: 30px;
        margin: 0 10px;
        vertical-align: text-bottom;
    }
}
</style>