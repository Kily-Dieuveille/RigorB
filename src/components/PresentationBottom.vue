<template>
  
    <footer>
        <div class="box-link">
            <div class="box-bottom">
                <h4>SHOP</h4>
                <a href="#">Femme</a>
                <a href="#">Homme</a>
                <a href="#">Bébé</a>
                <a href="#">Enfant</a>
                <a href="#">Acceuil</a>
                <a href="#">Promotion</a>
            </div>
            <div class="box-bottom">
                <h4>CORPORATE INFO</h4>
                <a href="#">Votre carrière chez RigorB</a>
                <a href="#">A propos de  RigorB</a>
                <a href="#">Developpement durable</a>
                <a href="#">Presse</a>
                <a href="#">Investor relations</a>
                <a href="#">Corporate governance</a>
            </div>
            <div class="box-bottom">
                <h4> HELP</h4>
                <a href="#">Service Client</a>
                <a href="#">Mon compte </a>
                <a href="#">Magasin</a>
                <a href="#">Mentions légales</a>
                <a href="#">confidentialité</a>
                <a href="#">Contact</a>
                <a href="#">Carte cadeau</a>
                <a href="#">Parametres des cookies</a>
            </div>
            <div class="box-bottom">
                <h4>INSCRIPTION</h4>
                <a href="#">Devenez membre & obtenez -10%</a>
                
                <button class="lire-la-suite"> LIRE LA SUITE &rarr </button>
            </div>
        </div>
        <div class="box-icon">
            <i class="fab fa-facebook"></i>
            <i class="fab fa-twitter"></i>
            <i class="fab fa-instagram"></i>
            <i class="fab fa-youtube"></i>
            <i class="fab fa-linkedin"></i>
        </div>
        <div class="box-text">
            <p>

        Le contenu de ce site est protégé par la loi du copyright et appartient à H & M Hennes & Mauritz AB. 
        Le concept du groupe H&M est de proposer mode et qualité au meilleur prix et de façon durable. 
        Depuis sa création en 1947, H&M est devenu l'un des principaux groupes de prêt-à-porter du monde.

            </p>

            <button class="lire-la-suite"> 
                LIRE LA SUITE
            </button>
        </div>
        <div class="box-logo">
            <img src="" alt="">
        </div>

    </footer>
</template>


<style scoped>
.box-icon
{
    display:flex;
    flex-direction: row;
    justify-content: center;

    margin-top: 10px;

}

.fab
{
    margin-left: 50px;
    margin-right: 50px;
}

footer
{

    background-color: beige;

}
.box-link
{
    display: flex;
    flex-direction: row;
    justify-content: space-around;

}
.box-bottom
{
    display:flex;
    flex-direction: column;
    font-family: Arial, Helvetica, sans-serif;
}

a 
{
    text-decoration: none;
    color:black;
    margin:13px;
}
.lire-la-suite
{ 
    border: none;
    background-color: beige;
}
.box-text 
 {
     margin:0 25% 0 25%;
     font-family: Arial, Helvetica, sans-serif;
 }
 

</style>
