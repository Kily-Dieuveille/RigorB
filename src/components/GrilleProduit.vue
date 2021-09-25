<template>
    <div class="grille-produit">
        <div class="box-image">
            <img v-for="lien of images" :key="lien" :src="lien" alt="">
        </div>
    </div>
</template>


<script>

export default {
    data:()=>{
        return {
            effectif:4,
            images:["./assets/Homme/H1.jpg","../assets/Homme/H1.jpg","C:/Users/NZIKI Dieuveille/Documents/azerty/rigorb/src/assets/Homme/H4.jpg"]
        }
    }
}
</script>

<style scoped>

</style>
