<template>
  <div v-if="gender === 'man'">
    <PresentationTop gender="man" />
    <Carousel gender="man" />
    <PrensentationBottom gender="man" />
  </div>
  <div v-else>
    <PresentationTop gender="woman" />
    <Carousel gender="woman" />
    <PrensentationBottom gender="woman" />
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
       gender: String
    }
}
</script> 