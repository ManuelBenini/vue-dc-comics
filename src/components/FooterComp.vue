<template>
  <footer>

    <div class="container mb-container">

      <ul>
        <li><h4>DC COMICS</h4></li>
        <li><a href="#">Characters</a></li>
        <li><a href="#">Comics</a></li>
        <li><a href="#">Movies</a></li>
        <li><a href="#">TV</a></li>
        <li><a href="#">Games</a></li>
        <li><a href="#">Videos</a></li>
        <li><a href="#">News</a></li>
        <li>
          <ul>
            <li><h4>SHOP</h4></li>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </li>
      </ul>


      <ul>
        <li><h4>DC</h4></li>
        <li><a href="#">Terms Of Use</a></li>
        <li><a href="#">Privacy policy (new)</a></li>
        <li><a href="#">Ad Choices</a></li>
        <li><a href="#">Advertising</a></li>
        <li><a href="#">Jobs</a></li>
        <li><a href="#">Subscriptions</a></li>
        <li><a href="#">Talent Workshops</a></li>
        <li><a href="#">CPSC Certificates</a></li>
        <li><a href="#">Ratings</a></li>
        <li><a href="#">Shop Help</a></li>
        <li><a href="#">Contact Us</a></li>
      </ul>

      <ul>
        <li><h4>SITES</h4></li>
        <li><a href="#">DC</a></li>
        <li><a href="#">MAD Magazine</a></li>
        <li><a href="#">DC Kids</a></li>
        <li><a href="#">DC Universe</a></li>
        <li><a href="#">DC Power Visa</a></li>
      </ul>

    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComp',
}
</script>

<style lang="scss" scoped>
footer{
  min-height: 300px;
  background-image: url('../assets/img/footer-bg.jpg');
  background-position: top;
  background-size: cover;
}
.mb-container{
  display: flex;
  background-image: url('../assets/img/dc-logo-bg.png');
  background-position: right center;
  background-repeat: no-repeat;
  padding: 30px 0;
  
}
ul{
  padding: 0 15px 0 0;
  li{
    h4{
      color: white;
      padding: 10px 0;
    }
    a{
      color: grey;
    }
    ul{
      margin: 0;
      padding: 5px 0;
    }
  }
}
</style>