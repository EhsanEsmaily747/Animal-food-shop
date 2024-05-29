<script setup>
    let datas = [
        {
            message:`I've never seen a cat food like this before. The nutritional balance is exceptional, and I've noticed remarkable improvements in the coat and energy levels of the cats I've recommended it to. It's a game-changer in feline nutrition.`,
            img:'/doctors/doctor1.png',
            name:'Dr. Sasharina',
            address: 'Girard, OH'
        },
        {
            message:`I've never seen a cat food like this before. The nutritional balance is exceptional, and I've noticed remarkable improvements in the coat and energy levels of the cats I've recommended it to. It's a game-changer in feline nutrition.`,
            img:'/doctors/doctor2.png',
            name:'Dr. Sara',
            address: 'Sacramento, CAL'
        },
        {
            message:`I've never seen a cat food like this before. The nutritional balance is exceptional, and I've noticed remarkable improvements in the coat and energy levels of the cats I've recommended it to. It's a game-changer in feline nutrition.`,
            img:'/doctors/doctor3.png',
            name:'Dr. Alex',
            address: 'Herat, AFG'
        },
        {
            message:`I've never seen a cat food like this before. The nutritional balance is exceptional, and I've noticed remarkable improvements in the coat and energy levels of the cats I've recommended it to. It's a game-changer in feline nutrition.`,
            img:'/doctors/doctor4.png',
            name:'Dr. Murphy',
            address: 'Girard, OH'
        },
    ]
</script>


<template>
  <div class="studies">
    <div class="study" v-for="data in datas">
      <span>,,</span>
      <p>I've never seen a cat food like this before. The nutritional balance is exceptional, and I've noticed remarkable improvements in the coat and energy levels of the cats I've recommended it to. It's a game-changer in feline nutrition.</p>
      <div class="profile-info">
        <img :src=data.img alt="" srcset="">
        <div>
          <h3>{{ data.name }}</h3>
          <h6>{{ data.address }}</h6>
        </div>
      </div>
    </div>
  </div> 

</template>

<style scoped>
    
.studies{
  position: relative;
  margin-block: 6rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
p{
  color: black;
  font-weight: 500;
  line-height: 1.5em;
}

.study{
position: relative;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  width: 20%;
  padding: 1rem 1.5rem;
  box-sizing: border-box;
  background: #fffbf5;

}
.profile-info{
  margin-top: 1.5em;
  display: flex;
  justify-content: flex-start;
  align-items: center;
}

.study span{
  position: absolute;
  left: 0;
  top: -40px;
  font-size: 8rem;
  letter-spacing: -20px;
  color: rgba(175, 175, 175, 0.541);
  transform: rotate(180deg) skewX(-4deg);
}

.profile-info img{
  width: 3.3rem;
  border-radius: 50%;
}

.profile-info div{
  height: 100%;
  margin-left: 20px;
  display: flex;
  flex-direction: column;
  align-items: baseline;
}

.profile-info div h3{
  font-weight: bolder;
  font-size: large;
}

.profile-info div h6{
  color: rgb(126, 126, 126);
}

</style>