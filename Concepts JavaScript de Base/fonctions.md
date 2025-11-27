Catégorie 1 : Concepts JavaScript de Base

sujet : Fonctions 

fonction : un bloc de code réutilisable ca veut dire au lieu d'écrire plusieurs fois le meme code , avec les fonctions ils est suffit de mettre le code dans une fonction et on l'appelle chaque fois qu'on en a besoin 

Déclaration de fonction : une fonction qui est nommé et tu peut l'appeler dans le code avant de la définie 

Expression de fonction : c'est une fonction assigné à une variable , il peut etre soit anonyme ou nommé , on ne peut pas l'appeler dans le code avant la définir 
 
syntaxe de déclaration de fonction : 
function nom-fonction(par1,par2){
    code a traiter 
}

syntaxe d'expression de fonction : 
const nom-var = function(par1, par2){
    code a traiter
}

quand on utilise la declaration d'une fonction : 
on utilise la déclaration de fonction quand on veut que la fonction soit disponible dans tous le fichier et quand on veut appeler la fonction avant la définir 

quand on utilise l'expression de fonction
quand on veux controler l'existance de fonction et tu veux éviter la disponibilité du fonction dans tous le fichier 


exemple de declaration de fonction : 
function calcule-prix() {
    return 100 * 2;
}

exemple de expression de fonction : 
const calcul-tva = function(prix) {
    return prix * 0.2;
};

fonction fléchée : c'est une maniére plus courte d'écrire des fonctions 

syntaxe de fonction fléchée 
const nom = (par1,par2) => {
    code a traiter
}     ===> au cas ou on a aucun paramétre on laisse les parenthése vide 

si ol a un seule paramaitre 
const nom = par => {
    code a traiter
}

quand utiliser les fonction fléchée 
on peut utiliser se genre de fonction quand on travaille sur une fonction courtes et simples 

exemple des fonction fléchée :

const addition = (a, b) => a + b;

console.log(addition(3, 4));

des exemples dans le contexte d'un système de réservation : 

function verifierDisponibilite(salle) {
    return salle.estLibre === true;
} 

on peut appeler cette fonction de n'importe ou dans le fichier car c'est une fonction de declaration 
un exemple de utilisation de cette fonction 

const salleA = { nom: "Salle A", estLibre: true };
console.log(verifierDisponibilite(salleA));

const calculerPrix = function(duree, prixParHeure) {
    return duree * prixParHeure;
};


ici la fonction ne peut pas etre appeler avant sa création car est une expression de fonction sa utilisation est comme suite 

console.log(calculerPrix(3, 100));

un exemple pour les fonction fléchée : 

const reserverSalle = (salle, nomClient) => {
    if (!salle.estLibre) {
        return "Salle déjà réservée !";
    }

    salle.estLibre = false;
    salle.client = nomClient;
    return `Salle réservée pour ${nomClient}`;
};

pour les appels des fonction fléchée est comme suite 

const salleB = { nom: "Salle B", estLibre: true };
console.log(reserverSalle(salleB, "Mohamed"));