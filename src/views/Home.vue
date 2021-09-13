<template>
  <div class="home">
    <div class="gender">
      <router-link class="vitrines" to="catalogue/Hommes">
      <img id=img_man src="../assets/image-pc.png" alt="" />
      </router-link>
      <router-link to="catalogue/Femmes">
      <img style="width:300px" src="../assets/femme-couleur-cheveux-colores-blonde-robe-rouge-fond-rouge-coloration-modele-femme-cheveux-blonds-couleur-cendre_91497-5261.jpg" alt="">
      </router-link>
    </div>
     <Carousel /> 

  </div>

 
  
</template>

<script>
import Carousel from "../components/Carousel.vue"

  export default {
    name:'Home',
    components:{
      Carousel
    }
  }
</script>

<style>
 .gender
 {
   display: flex;
   flex-direction: row;
   justify-content: space-between;
   justify-content: space-around;
   background-color:rgba(150, 66, 66, 0.836);
 }

 #img_man{
   width: 600px;
   height: 450px;
 }

.vitrines
{
  width:300px;
  min-height: 200px;
  border:1px solid black;
  display: flex;
  justify-content: center;
  overflow: hidden;
  
}
</style>