<template>
  <main>
    <div class="container mb-container">
     <h4>--- Content goes here ---</h4> 
    </div>
    
    </main>
</template>

<script>
export default {
  name: 'MainComp'
}
</script>

<style lang="scss" scoped>
main{
  background-color: #1c1c1c;
  .mb-container{
    min-height: 150px;
    display: flex;
    align-items: center;
    color: white;
  }
}
</style>