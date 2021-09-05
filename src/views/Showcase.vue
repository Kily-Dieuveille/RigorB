<template>
  <div v-if="gender === 'man'">
    <PresentationTop gdr="man" />
    <Carousel gdr="man" />
    <PrensentationBottom gdr="man" />
  </div>
  <div v-else>
    <PresentationTop gdr="woman" />
    <Carousel gdr="woman" />
    <PrensentationBottom gdr="woman" />
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
    props:{
        gdr: String
    }
}
</script> 