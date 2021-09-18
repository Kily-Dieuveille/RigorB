<template>
{{genre=$route.params.gender}}

  <div v-if="genre==='Hommes'">

    <PresentationTop/>
    <Carousel gender="man"/>
    <PrensentationBottom/>
    
  </div>

  <div v-else>

    <PresentationTop/>
    <Carousel gender="woman"/>
    <PrensentationBottom/>

  </div>
  
</template>

<script>
import PresentationTop from '@/components/PrensentationTop.vue'
import Carousel from '@/components/Carousel.vue'
import PrensentationBottom from '@/components/PresentationBottom.vue'

export default {
    name: "showcase",
    components: {
        PresentationTop,
        PrensentationBottom,
        Carousel,

    },
    data: ()=>{
      return {
        genre:''
      }
    }
}
</script> 