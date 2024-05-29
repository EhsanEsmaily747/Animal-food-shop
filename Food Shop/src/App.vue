
<script setup>
  import { ref, computed } from 'vue';
  import NavBar from './components/NavBar.vue'
  import HeroText from './components/heroText.vue'
  import HeroIMG from './components/HeroIMG.vue'
  import Studies from './components/Studies.vue'
  import Angry from './components/Angry.vue'


</script>


<template>
  <div>
    <NavBar></NavBar>
  </div>
  
  <main>
    <div>
      <HeroText></HeroText>
    </div>
    
    <div>
      <HeroIMG></HeroIMG>
    </div>
  </main>
  <div>
    <div>
      <p class="sub-title">Veternarians go bonkers for our tasty kitty formula.</p>
    </div>
  <Angry />
  </div>
  <Studies></Studies>
</template>

<style scoped>
main{
  margin-block: 140px;
  display: flex;
  box-sizing: border-box;
}
main div{
  width: 50%;
}

.sub-title{
  width: 60%;
  margin-inline: auto;
  margin-top: 11rem;
  letter-spacing: -3px;
  font-size: 55px;
  font-weight: bold;
  text-align: center;
}

</style>
