<template>

  <div v-if="$route.params.gender==='Hommes'">

    <PresentationTop/>
    <Carousel gender="man"/>
    <GrilleProduit/>
    <PrensentationBottom/>
    
  </div>

  <div v-else>

    <PresentationTop/>
    <Carousel gender="woman"/>
    <GrilleProduit/> 
    <PrensentationBottom/>

  </div>
  
</template>

<script>
import PresentationTop from '@/components/PrensentationTop.vue'
import Carousel from '@/components/Carousel.vue'
import PrensentationBottom from '@/components/PresentationBottom.vue'
import GrilleProduit from '@/components/GrilleProduit.vue'

export default {
    name: "showcase",
    components: {
        PresentationTop,
        PrensentationBottom,
        Carousel,
        GrilleProduit

    },
    data: ()=>{
      return {
        genre:''
      }
    }
}
</script> 