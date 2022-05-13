<template>
  <header>

  <div class="container mb_container d-flex align-items-center justify-content-between h-100">

    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="">
    </div>

    <nav>
      <ul class="d-flex align-items-end">
        <li :class="{'active' : page.isActive}" v-for="(page, index) in pagesCategories" :key="`page-${index}`"><a :href="page.href">{{page.name.toUpperCase()}}</a></li>
      </ul>
    </nav>

  </div>


  </header>
</template>

<script>
export default {
  name: 'HeaderComp',
  data(){
    return{
      pagesCategories: [
        {
          name: 'Characters',
          href: '#',
          isActive: false
        },
        {
          name: 'Comics',
          href: '#',
          isActive: true
        },
        {
          name: 'Movies',
          href: '#',
          isActive: false
        },
        {
          name: 'TV',
          href: '#',
          isActive: false
        },
        {
          name: 'Games',
          href: '#',
          isActive: false
        },
        {
          name: 'Collectibles',
          href: '#',
          isActive: false
        },
        {
          name: 'Videos',
          href: '#',
          isActive: false
        },
        {
          name: 'Fans',
          href: '#',
          isActive: false
        },
        {
          name: 'News',
          href: '#',
          isActive: false
        },
        {
          name: 'Shop',
          href: '#',
          isActive: false
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

  @import "../assets/style/variables.scss";

  header{
    height: 100px;
  }
  .logo{
    height: 70px;
    img{
      width: 100%;
      height: 100%;
    }
  }
  ul{
    list-style: none;
    li{
      border-bottom: 4px solid white;
      &:hover,
      &.active{
        border-color: $primary-color;
      &:hover a{
        color: $primary-color;
      }
      }
      a{
        display: inline-block;
        margin: 44px 5px;
        padding: 0px 5px;
        color: black;
      }
    }
    
  }
</style>