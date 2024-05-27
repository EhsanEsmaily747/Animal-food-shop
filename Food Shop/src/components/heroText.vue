<template>
    <div class="hero">
      <h1>Your cat will go <div><img src="/Bonkers..png " srcset=""></div></h1>
      <p>..for the world’s best testing cat food, sourced with only the finest ingredients.
         Made with love from the heart of Mississippi.</p>
    </div>
    <button>Get Bonkers</button>
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

button{
  width: 180px;
  height: 50px;
  font-size: 20px;
  margin-top: 3.5rem;
  font-weight: bold;
  background-color: var(--primary-color);
  border: none;
  border-radius: 6px;
  cursor: pointer;
  box-sizing: border-box;
  transition: border ease 100ms ;
}

button:hover{
  border: solid 2px black;
}

</style>