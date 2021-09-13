<template>
    <div id="section">
        <h1> La Mode à votre plaisir </h1>
        <h2>Vous êtes à l'honneur </h2>
        <div class="carousels">
            <div class="carousel">
                <div class="carousel-box" id="box1" @click="run()">
                    
                    <img src="..\assets\Femme\F1.jpg" alt="">                    
                    <img src="..\assets\Femme\F2.jpg" alt="">  
                    <img src="..\assets\Femme\F4.jpg" alt="">                    
                    <img src="..\assets\Femme\F7.jpg" alt="">   
                                                
                  
                </div>

            </div>
            <div class="carousel" >
                <div class="carousel-box" id="box2" @click="run()">

                    <img src="..\assets\Homme\H1.jpg" alt="">                    
                    <img src="..\assets\Homme\H3.jpg" alt="">                    
                    <img src="..\assets\Homme\H4.jpg" alt="">                    
                    <img src="..\assets\Homme\H2.jpg" alt="">                    
                
                </div>
            </div>
            <div class="carousel">
                <div class="carousel-box" id="box3" @click="run()">
                    
                    <img src="" alt="">                    
                    <img src="" alt="">                    
                    <img src="" alt="">                    
                    <img src="" alt="">                    
                    <img src="" alt="">   
                
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Carousel',
    props:['gender'],
    
    data: ()=>{
        return {
            imgs_box1:[],
            imgs_box2:[],
            imgs_box3:[],
            
            idx1:0,
            idx2:0,
            idx3:0,
        }

    },
    methods:
    {
        run(){

            this.imgs_box1=document.querySelectorAll("#box1 img");            
            this.imgs_box2=document.querySelectorAll("#box2 img");
            this.imgs_box3=document.querySelectorAll("#box3 img");

            const box1 = document.getElementById("box1");
            const box2 = document.getElementById("box2");
            const box3 = document.getElementById("box3");

            if(this.idx1>this.imgs_box1.length-1){
                this.idx1=0;
            } 
            if(this.idx2>this.imgs_box2.length-1){
                this.idx2=0;
            } 
            if(this.idx3>this.imgs_box3.length-1){
                this.idx3=0;
            }

            this.idx1++
            this.idx2++
            this.idx3++

            box1.style.transform ="translateX("+-this.idx1*470+"px)";
            box2.style.transform ="translateX("+-this.idx2*470+"px)";
            box3.style.transform ="translateX("+-this.idx3*470+"px)";

            console.log("c'est fait !");
            

        }
    }

}



</script>

<style scoped>
#section
{

    background-color: bisque;
}
.carousels
{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    justify-content:space-around;
    align-items: center;

    background-color: bisque;
}


 img
 {
    object-fit: cover;
    width: 470px;
    height: 570px;
 }

.carousel-box
{
    display: flex;
    flex-direction: row;
    width:2000px;
    transition: transform linear 0.1s;
    transform: translateX(0px);
}
.carousel
{
    overflow: hidden;
    width: 470px;
    height:570px;

    box-shadow: 2px 2px 5px rgba(0, 0, 0,0.3);

}

</style>