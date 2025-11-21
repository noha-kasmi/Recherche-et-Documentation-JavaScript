Catégorie 2 : Manipulation du DOM 
sujet : DOM (document object model)

définition de dom : dom c'est la représentation html dans le javascript , il transferme le fichier html lit par le navigateur en une structures d'objets 

quand utiliser DOM? 
on utilise le dom pour modifier la page web pendant qu'elle est affiché 

Exemple simple : 
dans ce exemple si on clique sur le bouton , le texte doit changer 

page html : 
<h1 id="titre">Bonjour</h1>
<button id="btn">Changer le texte</button>

page js : 
const titre = document.getElementById("titre");
const btn = document.getElementById("btn");

btn.addEventListener("click",() => {
    titre.textContent = "bonjour , le texte est changé ";
});