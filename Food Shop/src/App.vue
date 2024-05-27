
<script setup>
  import NavBar from './components/NavBar.vue'
  import HeroText from './components/heroText.vue'
  import HeroIMG from './components/HeroIMG.vue'
</script>


<template>
  <div>
    <NavBar></NavBar>
  </div>
  
  <main>
    <div style="width: 50%;">

      <HeroText></HeroText>
    </div>
    
    <div style="width: 50%;">
      <HeroIMG></HeroIMG>
    </div>
  </main>
</template>

<style scoped>
main{
  margin-top: 140px;
  display: flex;
  box-sizing: border-box;
}

</style>
