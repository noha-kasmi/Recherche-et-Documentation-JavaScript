Catégorie 1 : Concepts JavaScript de Base

Variables : se sont des conteneurs pour stocker les données 

La définitions de Var , let et const : 
 pour 'let' c'est une variable modifiable ca veut dire qu'on peut la changer ,
 à propos de 'const' , c'est une constante non modifiable docn on peut pas la changer , 
 'var' , c'est une ancienne variable on ne l'utilise plus . 

la différence entre var , let et const : 
var peut etre redéclaré et changer et meme si tu le mets dans un if , il reste accessible dehors . 
let ne peut pas etre redéclaré mais peut etre modifié et il reste dans le bloc ou il a été crée
const ne peut pas etre redéclaré et ne peut pas etre changer et il reste dans le bloc ou il a été crée 

 Syntaxe de var : 
 var nom-variable = valeur;

 Syntaxe de let : 
 let nom-variable = valeur;

 Syntaxe de const : 
 const nom-variable = valeur; 

 quand utiliser var? 
 on ne l'utilise pas car il peut créer des bugs

 quand utiliser let? 
 on l'utilise quand la valeur va changer 

 quand utiliser const? 
 on l'utilise quand la valeur va reste stable 

 exemple de var : 
 var nom = "Noha";
 var prenom ="Kasmi";
 console.log(nom);  --> résultat :Noha

 exemple de let : 
 if (true){
 let message = "bonjour ! ";
 console.log(message);  -->il s'affiche ici le bonjour 
 }
 console.log(message); --> mais ici il ne s'affiche pas car let reste    seulement dans le bloc 

 exemple de const : 
 if (true) {
 const message = "Bienvenue !";
 console.log(message); 
}
 console.log(message);