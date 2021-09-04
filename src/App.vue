<template>

  <header>
    <div id="menu">
      <router-link to="catalogue/Hommes" id="man"> MAN </router-link>
      <span class="separateur_verticale"></span>
      <router-link to="catalogue/Femmes" id="woman"> WOMAN </router-link>
    </div>
  </header>

  <router-view></router-view>
</template>

<script>


</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}


.separateur_verticale
{
  display: inline-block;
  border-left: 2px solid black;
  height: 15px;
}
</style>
