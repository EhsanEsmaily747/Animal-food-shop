
<script setup>
  import { ref, computed } from 'vue';
  import NavBar from './components/NavBar.vue'
  import HeroText from './components/heroText.vue'
  import HeroIMG from './components/HeroIMG.vue'
  import Studies from './components/Studies.vue'
  import Angry from './components/Angry.vue'
  import Facts from './components/Facts.vue'
  import Button from './components/Button.vue'

</script>


<template>
  <div>
    <NavBar></NavBar>
  </div>
  
  <main>
    <div>
      <HeroText/>
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
  <Studies/>

  <div >
    <Facts/>
  </div>  

  <div class="last-section">
    <div>
      <h1 class="logo">friskay</h1>
      <h1 class="text">Are you ready to <br>go bonkers?</h1>
    </div>
    <div>
      <Button/>
    </div>
  </div>

  <footer>
      <NavBar class="nav"/>
  </footer>
</template>

<style scoped>
footer{
  height: 15vh;
  position: relative;
}
footer .nav{
  position: relative;
  top: 50%;
  transform: translateY(-50%);
}
footer::before{
  content: '';
  background-color: #FEECCA;
  position: absolute;
  width: 100vw;
  height: 100%;
  left: -120px;
  z-index: -1;
}

.logo{
  font-size: 28px;
  font-weight: 500;
  margin-bottom: 10px;
}
div .text{
  font-size: 60px;
  line-height: 1.2em;
  letter-spacing: -3px;
}
.last-section{
  gap:5rem;
  height: 85vh;
  display: flex;
  justify-content: center;
  align-items: center;
}


.last-section>div{
  width: 50%;
  text-align: right;
}
.last-section>div:first-child{
  box-sizing: border-box;
}

.last-section>div:last-child{
  text-align: left;
}

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
