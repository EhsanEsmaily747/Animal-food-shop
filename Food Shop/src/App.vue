
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
  
      <div class="main-container">
        <div class="guy"></div>
      </div>
  </div>

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

.main-container{

  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 550px;
  width: 100%;
  text-align: center;
  background-image: url(/Group\ 15.png);
  background-repeat: repeat-x;
  background-position: center;
  /* background-size: contain; */
  animation: steping 1s ease-in;
}
.main-container::before{
  content: '';
  width: 35%;
  aspect-ratio: 1;
  border-radius: 50%;
  position: absolute;
  background-color: white;
  z-index: -1;
  
}
.main-container::after{
  content: '';
  width: 25%;
  aspect-ratio: 1;
  border-radius: 50%;
  position: absolute;
  z-index: -1;
  background-color: #FFEBC3;
}

.guy{
  width: 28%;
  position: relative;
  top: 7vh;
  aspect-ratio: 1;
  background-image: url(Ellipse\ 3.png);
  background-size: contain;
}


</style>
