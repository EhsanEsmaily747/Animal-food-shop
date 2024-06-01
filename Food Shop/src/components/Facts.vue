<template>
    <div class="container">
    <div class="img"><img src="/bowl 1.png" alt="" srcset=""></div>
    <div class="facts">
      <div class="fact">
        <div class="label">Fact 1</div>
        <div class="text">Free from artificial colors, flavors, and preservatives, our cat food offers a natural and nutritious diet for your feline friend.</div>
      </div>
      <div class="fact">
        <div class="label">Fact 1</div>
        <div class="text">Formulated with prebiotics and probiotics, this cat food aids in digestion and supports a balanced gut microbiome.</div>
      </div>
      <div class="fact">
        <div class="label">Fact 1</div>
        <div class="text">Enriched with omega-3 and omega-6 fatty acids, it promotes a shiny coat and healthy skin, making it ideal for cats with sensitive skin</div>
      </div>
      <div class="fact">
        <div class="label">Fact 1</div>
        <div class="text">Packed with high-quality protein, our new cat food supports strong muscles and a healthy heart in cats of all ages.</div>
      </div>
    </div>
  </div>
</template>


<style scoped>
    
.facts{
  display: flex;
  position: relative;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}

.fact{
  width: 40%;
  margin-bottom: 80px;
}

.fact .label{
  background: rgba(255, 255, 255, 0.377);
  width: fit-content;
  position: relative;
  top: -30px;
  padding: 5px 10px;
  border-radius: 6px;
  font-size: 23px;
  font-weight: bold;
  transform: rotate(-18deg);
}
.fact .text{
  width: fit-content;
  font-size: 22px;
  line-height: 1.3em;
}


.container{
  display: flex;
  align-items: flex-end;
  height: 95vh;
  margin-top: 30vh;
  position: relative;
}
.container::before{
  content: '';
  width: 100vw;
  height: 100%;
  position: absolute;
  left: -120px;
  background: var(--secondary-color);
  z-index: -1;
}

.container .img{
  position: absolute;
  top: -22%;
  left: 50%;
  transform: translateX(-50%);
}


</style>