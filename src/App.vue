<template>
  <div id="app">
    <div class="formContainer">
      <MenuPage/>
      <NavbarPage/>
      <HomePage/>
      <SubnavPage/>
    </div>
  </div>
</template>

<script>

import "./themify-icons/themify-icons.css"
import MenuPage from "./components/MenuPage.vue"
import NavbarPage from "./components/NavbarPage.vue"
import HomePage from "./components/HomePage.vue"
import SubnavPage from "./components/SubnavPage.vue"


export default {
  name: 'App',
  components: {
    MenuPage,
    NavbarPage,
    HomePage,
    SubnavPage
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: flex;
  justify-content: center;
  height: 98vh;
}
li{
  list-style-type: none;
}
a{
  text-decoration: none;
}
ul{
  padding:0 0 ;
}
.formContainer{
  /* background: url('./assets/imgs/background.jpg'); */
  /* background-color: brown; */
  width: 900px;
  height: 76%;
  margin: auto;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: row;
  border-radius: 16px;
}
</style>
