<template>
    <div style="position: relative; width: 100%;">
        <div class="pic">
          <div class="hero-pic"></div>    
      </div>
    </div>
</template>


<style scoped>
  .pic{
    /* height: 100vh;   */
    position: absolute;
    width: 850px;
    z-index: -1;
    right: -10%;
    top: -3vh;
  }
  .pic::before{
    content: '';
    position: absolute;
    top: 50%;
    left: 0;
    z-index: -1;
    aspect-ratio: 1;
    width: 106%;
    border-radius: 50%;
    background: white;
    transform: translate(-3%,-50%);
    
  }
  
.pic::after{
  z-index: -1;
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
  aspect-ratio: 1;
  border-radius: 50%;
  width: 480px;
  background-color: #FFEBC3;
}

.hero-pic{
  position: relative;
  left: 50%;
  top: 50%;
  transform: translate(-50%,0);
  width: 500px;
  height: 450px;
  background-image: url(/cat\ 1.png);
  background-repeat: no-repeat;
  background-size: cover;
  animation: moving 3500ms ease-in-out infinite ;
}

@keyframes moving {
  0%{
    transform: translate(-50%,0);
  }
  50%{
    transform: translate(-57%, -7%);
  }
  100%{
    transform: translate(-50%, 0);
  }
}

</style>