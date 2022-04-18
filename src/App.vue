<script setup>
import Menu from "./components/Menu.vue"
import KeyResultBoard from "./components/KeyResultBoard.vue"

</script>

<template>
    <div class="App">
      <div class="menu">
        <Menu />
      </div>
      <div class="content">
        <KeyResultBoard />
      </div>
    </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700;900&display=swap');
  *{
    margin: 0;
    padding: 0;
    text-decoration: none;
    list-style: none;
    font-family: 'Roboto', sans-serif;
  }
  .App{
    display:flex;
  }
  .menu{
    display:flex;
    justify-content: center;
    box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 14px;
    width: 20vw;
    background-color: #FAFAFA;
    height: 100vh;
    border-radius: 0 20px 20px 0;
  }
  .content{
    width: 80vw;
    display: flex;
    justify-content: center;
    align-items: center
  }
</style>
