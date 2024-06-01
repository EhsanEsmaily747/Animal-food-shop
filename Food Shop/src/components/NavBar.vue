

<template>
      <nav>
    <div>
      <h1 class="logo">friskay</h1>
      <p class="page">HOME</p>
    </div>
    <div>
      <ul>
        <li>Our Food</li>
        <li>Studies</li>
        <li>Ingredients</li>
        <li>FAQ</li>
      </ul>
    </div>
  </nav>
</template>

<style scoped>
     nav,nav div , nav div ul{
    display: flex;
    flex-direction: row;
  }

  nav {
    justify-content: space-between;
  }
  nav div:nth-child(1) {
    width: 200px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .logo{
    font-size: 28px;
    border-right: solid 1px gray;
    padding-right: 30px;
  }
  .page{
    color: gray;
    font-size: 15px;
  }

  nav div:nth-child(2){
    width: 50%;
    font-weight: bold;
  }

  ul{
    width: 100%;
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }

  ul li{
    margin-left: 65px;
    font-weight: 600;
    font-size: 18px;
    cursor: pointer;
  }

  ul li:hover{
    color: var(--primary-color);
  }
</style>