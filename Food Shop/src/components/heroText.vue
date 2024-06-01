<script setup>
  import Button from './Button.vue'
</script>

<template>
    <div class="hero">
      <h1>Your cat will go <div><img src="/Bonkers..png " srcset=""></div></h1>
      <p>..for the world’s best testing cat food, sourced with only the finest ingredients.
         Made with love from the heart of Mississippi.</p>
    </div>
    <div style="margin-top: 3.5rem;">
      <Button/>
    </div>
</template>


<style scoped>


.hero h1{
  font-size: 70px;
  margin-bottom: 25px;
}

h1 div{
  margin-left: 5px;
}

p{
  font-size: 22px;
  font-weight: 300;
  width: 80%;
}

</style>