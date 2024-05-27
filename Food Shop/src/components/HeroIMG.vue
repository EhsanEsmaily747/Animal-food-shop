<template>
    <div>
        <div class="pic">
        <div class="c-out">
          <div class="c-in">
            <div class="hero-pic"></div>
          </div>
        </div>
      </div>
    </div>
</template>


<style scoped>
  .pic{
    position: absolute;
    width: 850px;
    z-index: -1;
    right: 0;
    top: 0;
  }
  .c-out{
    position: relative;
    aspect-ratio: 1;
    border-radius: 50%;
    background: white;
    display: flex;
    justify-content: center;
    align-items: center;
    transform: translate(-7%,-5%);
    
  }
  
.c-in{
  aspect-ratio: 1;
  border-radius: 50%;
  width: 57%;
  background-color: #FFEBC3;
}

.hero-pic{
  width: 501px;
  height: 459px;
  background-image: url(/cat\ 1.png);
  background-repeat: no-repeat;
  background-size: cover;
  animation: moving 3500ms ease-in-out infinite ;
}

@keyframes moving {
  0%{
    transform: translate(30px,10px);
  }
  50%{
    transform: translate(-30px, -10px);
  }
  100%{
    transform: translate(30px, 10px);
  }
}

</style>