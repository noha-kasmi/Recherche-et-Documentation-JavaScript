sujet : Séléction d'élément 

getElementById("") : méthode js pour seléctionner un élément html avec son attribut id  
cette méthode  renvoie un seul élément car le id est unique 

syntaxe : 
document.getElementById("le-id");

cas d'utilisation: 
on utilise cette méthode quand on veut récupérer ou modifier un élément précis dans ta page 

exemple : 
const titre = document.getElementById("titre");

querySelector("") : méthode js pour séléctionner le premier élément qui est correspondant à un sélécteur (id , classe,balise html , attribut etc ....)

syntaxe:
document.querySelector("");

cas d'utilisation : 
on l'utilise si on veut pas séléctionner un élément avec le id 

exemple : 
page html :
<p class="message">Bonjour</p>

page js :
const msg = document.querySelector(".message");
console.log(msg.textContent); -->class css

const msg = document.querySelector("p"); --> balise html 

un exemple pour un sélécteur complexe 

page html : 
<div class="menu">
   <p class="item active">Accueil</p>
   <p class="item">Contact</p>
</div>

page js :
const itemActif = document.querySelector(".menu .item.active");

un exemple pour travailler sur un bouton 

page html : 
<button class="btn-acheter">Acheter</button>

page js :
const btn = document.querySelector(".btn-acheter");

btn.addEventListener("click", () => {
    alert("Produit ajouté !");
});
