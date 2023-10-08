#JAVASCRIPT
==============

![Définition JS](DéfinitionJS.png)

##Déclarer une variable :
----------------------

####var, let où const
---------------------

String :
--------

var nom = 'Hayete';

Number :
--------

var number = 23;

Déclarer un objet =
-------------------

var ob = {};

Déclarer un tableau :
---------------------

var fruits = ['pomme', 'poire', 'bananne', 'cerise']
var annonce = 'bonjour il y a des ' + fruits[0] + 's dans le rayon fruit'

Obtenir l'affichage :
---------------------

console.log(fruits[0],fruits[2])
console.log(annonce)

Chercher par l'index :
---------------------

exemple:
var fruits = ['pomme', 'poire', 'bananne']
var annonce = 'bonjour il y a des ' + fruits[0] + 's dans le rayon fruit'
console.log(annonce)
console.log(fruits[0]);//simple
pomme
console.log(fruits[0],fruits[2])//multiple
bonjour il y a des pommes dans le rayon fruit
//à noter nous avons ajouter un s car pomme était au singulier//
pomme
bananne

Rechercher par l'indexOf() :
---------------------------

var indexElement = fruits.indexOf('banane'); // Trouve l'index de "banane"

Remplacement d'un élèment :
---------------------------

fruits[1] = 'fraise';
console.log(fruits);//on obtient ainsi Fraise

Longueur de la liste :
----------------------

console.log(fruits.length);

Booléan :
--------

var estetudiant = ('true');
console.log(estetudiant);

Inversion :
-----------

var estetudiant = !('true');
console.log(estetudiant);

Clé/Valeurs :
-------------

var couleurs = { Ciel: "Bleu", Feu: "Rouge", Foret: "Vert" };
console.log(couleurs);

Accèder aux valeurs :
---------------------

console.log(couleurs.Ciel);//le "." est utilisé pour appeller

Modification :
--------------

couleurs.Feu = 'Orange';
console.log(couleurs.Feu);

Afficher plusieurs variables :
-----------------------------

var un = 'Je';
var deux = 'suis';
var trois = 'fatiguée.'
var quatre = (un + ' ' + deux + ' ' + trois);
console.log(quatre);

Déterminé type de variable :
----------------------------

console.log(typeof age);

calcul en pourcentage :
-----------------------

//Méthode de Darine
var prixarticle = 25;
var remise = 20;
console.log(prixarticle * (1 - remise / 100));

var prixArticle = 100;
var remise = 25;
var montantRemise = (prixArticle * remise) / 100;
var prixApresRemise = prixArticle - montantRemise;
console.log(prixApresRemise);

Concaténer avec des variables :
-------------------------------

var cinq = "J'ai";
var six = 35;
var sept = "dollars";
var huit = "et"
var neuf = "40 cents."
var newTexte = (cinq + ' ' + six + ' ' + sept + ' ' + huit + ' ' + neuf);
console.log(newTexte);

//Méthode d'Eddine 
var liste = ["J'ai", 35, "dollars", "et", "40 cents."];
var newliste = ''.concat(...liste);
console.log(newliste);

Variable conditionnelle :
-------------------------

//Déclarez une variable jour et assignez-lui un jour de la semaine ("Lundi", "Mardi", etc.).
//Affichez un message dans la console en fonction du jour(par exemple, "Bon lundi !" si le jour est "Lundi").
//Contrainte: Utilisez une instruction conditionnelle pour déterminer le message à afficher

var jour = "Lundi";
if (jour === "Lundi") {
    console.log("Bon lundi !");
} else if (jour === "Mardi") {
    console.log("Bon mardi !");
} else if (jour === "Mercredi") {
    console.log("Bon mercredi !");
} else if (jour === "Jeudi") {
    console.log("Bon jeudi !");
} else if (jour === "Vendredi") {
    console.log("Bon vendredi !");
} else if (jour === "Samedi") {
    console.log("Bon samedi !");
} else if (jour === "Dimanche") {
    console.log("Bon dimanche !");
} else {
    console.log("Jour non valide.");
}

//Dans cet exercice, j'ai déclaré la variable jour et je lui ai attribué la valeur "Lundi".
//Ensuite, j'ai utilisé une instruction conditionnelle if-else pour déterminer le message à
//afficher en fonction de la valeur de jour.Si jour est égal à "Lundi", le message "Bon lundi !"
//sera affiché.Il est possible adapter ce code en changeant la valeur de la variable jour
//pour afficher un message différent en fonction du jour qu'on souhaite.

Conversion : 
-----------

//Pour convertir une chaîne de caractères en une liste de mots en JavaScript,
//on peut utiliser la méthode split().Cette méthode découpe la chaîne en fonction 
//d'un délimiteur (par exemple, un espace) et renvoie un tableau contenant les mots individuels. Voici comment faire :

var chaineDeCaracteres = "Ceci est une phrase à convertir en liste de mots";
var listeDeMots = chaineDeCaracteres.split(" ");
console.log(listeDeMots);

//Dans cet exemple, nous avons une chaîne de caractères chaineDeCaracteres.
//Nous utilisons la méthode split(" ") pour diviser la chaîne à chaque espace,
//créant ainsi un tableau listeDeMots contenant les mots individuels.

joint :
-------

var listeDeMots = ["Bonjour", "à", "tous", "les", "développeurs", "web."];
var chaineResultat = listeDeMots.join(" ");
console.log(chaineResultat);

//Ce code prend la liste listeDeMots et utilise la méthode join()
//pour les fusionner en une seule chaîne en les séparant par des espaces.
//On peut remplacer l'espace " " dans join() par n'importe quel caractère qu'on souhaite utiliser comme séparateur entre les mots.

Accéder aux listes :
-------------------

//Énoncé: Affichez les deux premiers et les deux derniers éléments d'une liste.
//Contrainte: Utilisez l'indexation pour accéder aux éléments.

var listeBis = ["Chapeau", "Gants", "Echarpe", "Pantalon", "Veste", "Robe", "Pull"];
var deuxPremiers = [listeBis[0], listeBis[1]];

// Les deux derniers éléments
var deuxDerniers = [listeBis[listeBis.length - 2], listeBis[listeBis.length - 1]];

// Affichage des résultats
console.log("Les deux premiers éléments : " + deuxPremiers);
console.log("Les deux derniers éléments : " + deuxDerniers);

Somme des listes :
-----------------

//Pour calculer la somme des éléments d'une liste en JavaScript, nous pouvons utiliser une boucle 
//for pour parcourir la liste et accumuler la somme.
// Liste d'éléments
var maNewListe = [1, 2, 3, 4, 5];

// Variable pour stocker la somme
var somme = 0;

// Parcourir la liste et accumuler la somme
for (let i = 0; i < maNewListe.length; i++) {
    somme += maNewListe[i];
}

// Afficher la somme
console.log("La somme des éléments de la liste est : " + somme);
//Ce code initialise une variable somme à zéro,
//puis utilise une boucle for pour parcourir la liste maListe
//et ajoute chaque élément à la somme.Enfin, il affiche la somme totale.


Mélange de type de données :
--------------------------

//En JavaScript, il existe plusieurs types de données, notamment :

//1-Number (Nombre) : Il représente à la fois les nombres entiers et les nombres décimaux (à virgule flottante). Par exemple, 3, 3.14.

//2-String (Chaîne de caractères) : Il représente du texte encadré par des guillemets simples (') ou doubles ("). Par exemple, "Bonjour", 'JavaScript'.

//3-Boolean (Booléen) : Il représente une valeur binaire, soit true (vrai) ou false (faux). 
//Il est couramment utilisé pour les conditions.Par exemple, true, false.

//4-Array (Tableau) : Il représente une collection ordonnée d'éléments, qui peuvent être de différents types. 
//Les éléments d'un tableau sont accessibles par leur index. Par exemple, [1, 2, 3], ['a', 'b', 'c'].

//5-Object (Objet) : Il représente une collection non ordonnée de paires clé-valeur. L
//es propriétés d'un objet sont accessibles par leur nom de clé. Par exemple, { nom: 'John', age: 30 }.

//6-Undefined (Non défini) : Il représente une variable ou une valeur qui n'a pas été initialisée. 
//En général, une variable est automatiquement initialisée à undefined si aucune valeur n'est attribuée.

//7-Null (Nul) : Il représente l'absence intentionnelle de valeur ou une valeur nulle.

//8-Symbol (Symbole) : Il représente une valeur unique qui peut être utilisée comme clé d'objet. 
//Il est principalement utilisé dans le contexte des propriétés d'objet.

//9-Function (Fonction) : En JavaScript, les fonctions sont également considérées comme des types de données. 
//Elles peuvent être définies et utilisées pour effectuer des actions ou des calculs spécifiques.

//10-Date (Date) : Il représente une date et une heure spécifiques.

//11-RegExp (Expression régulière) : Il représente une expression régulière utilisée pour la recherche et la manipulation de chaînes de caractères.

//12-Map (Mappe) et Set (Ensemble) : Ce sont des structures de données introduites dans ECMAScript 6 (ES6) 
//pour stocker des collections de données.Map associe des clés à des valeurs, tandis que Set stocke des valeurs uniques.

//Ces différents types de données permettent de représenter et de manipuler diverses informations dans JavaScript, 
//ce qui en fait un langage très flexible et puissant.
var premier = ("Rien à ajouter", 55, [1, 2, 3]);


Retrait d'élment d'une liste splice:
------------------------------------

//Pour retirer un élément spécifique d'une liste en JavaScript en utilisant une méthode de liste, 
//vous pouvez utiliser la méthode splice().Voici comment retirer un élément spécifique, par exemple, "banane", de la liste fruits:

var indexElementARetirer = fruits.indexOf('banane'); // Trouve l'index de "banane"
if (indexElementARetirer !== -1) {
    fruits.splice(indexElementARetirer, 1); // Retire 1 élément à l'index trouvé
}

console.log(fruits); // La liste de fruits sans "banane"
//Dans ce code, nous utilisons indexOf() pour trouver l'index de l'élément que nous voulons retirer,
//puis nous utilisons splice() pour retirer cet élément de la liste.

//Après l'exécution de ce code, la liste fruits ne contiendra plus l'élément "banane".

//Pour retirer un élément d'une liste en JavaScript, vous pouvez utiliser la méthode pop() 
//pour supprimer le dernier élément de la liste ou la méthode shift() 
//pour supprimer le premier élément de la liste.Voici comment vous pouvez faire cela:

// Utilisation de pop() pour retirer le dernier élément
fruits.pop();
console.log(fruits); // La liste de fruits sans le dernier élément

//Pour retirer le premier élément de la liste (pomme dans ce cas) en utilisant shift() :
fruits.shift();
console.log(fruits); // La liste de fruits sans le premier élément
//Choisissez la méthode qui correspond à l'élément que vous souhaitez retirer (dernier?premier, où n'importe où) en fonction de votre besoin.


//Pour retirer un élément spécifique d'une liste en JavaScript en utilisant une méthode de liste,
//vous pouvez utiliser la méthode splice().Voici comment retirer un élément spécifique, par exemple, "banane", de la liste fruits:


Nombre aléatoire random :
------------------------

//Pour générer un nombre aléatoire en JavaScript en respectant la contrainte d'utiliser une fonction mathématique native, 
//vous pouvez utiliser la fonction Math.random().Voici comment vous pouvez le faire:


// Utilisation de Math.random() pour générer un nombre aléatoire entre 0 (inclus) et 1 (exclus)
let nombreAleatoire = Math.random();
console.log(nombreAleatoire); // Affiche le nombre aléatoire généré
//La fonction Math.random() génère un nombre décimal aléatoire compris entre 0 (inclus) et 1 (exclus). 
//Si vous souhaitez obtenir un nombre aléatoire dans une plage différente, 
//vous pouvez utiliser des opérations mathématiques pour ajuster la plage et le type de nombre (entier ou décimal) 
//selon vos besoins.Par exemple, pour obtenir un nombre entier aléatoire entre 1 et 100, vous pouvez faire ceci:


let nombreAleatoireEntier = Math.floor(Math.random() * 100) + 1;
console.log(nombreAleatoireEntier); // Affiche un nombre entier aléatoire entre 1 et 100
//Ici, Math.floor() est utilisé pour arrondir le résultat à un nombre entier,
//et nous ajoutons 1 pour obtenir une plage de 1 à 100. Vous pouvez ajuster ces valeurs en fonction de vos besoins spécifiques.

Arrondir avec math.round:
-------------------------

// Nombre à virgule
let nombreAVirgule = 5.67;

// Utilisation de Math.round() pour arrondir à l'entier le plus proche
let entierArrondi = Math.round(nombreAVirgule);

console.log(entierArrondi); // Affiche l'entier arrondi le plus proche
//La fonction Math.round() prend un nombre à virgule en entrée et renvoie l'entier le plus proche.
//Si la partie décimale est égale ou supérieure à 0.5, l'entier sera arrondi vers le haut.
//Si la partie décimale est inférieure à 0.5, l'entier sera arrondi vers le bas.

//Dans l'exemple ci-dessus, si nombreAVirgule est de 5.67, alors entierArrondi sera de 6,
//car 5.67 est plus proche de 6 que de 5. Si nombreAVirgule était de 5.34, alors entierArrondi serait de 5.

Conversion de type parsFloat/parseInt:
-------------------------------------

//Pour convertir une chaîne de caractères en nombre en utilisant une fonction native de JavaScript, 
//vous pouvez utiliser la fonction parseFloat() pour obtenir un nombre à virgule flottante ou la fonction parseInt() 
//pour obtenir un nombre entier.Voici comment vous pouvez faire cela:

//Convertir en nombre à virgule flottante en utilisant parseFloat() :
// Chaîne de caractères
let truc = "3.14";

// Utilisation de parseFloat() pour la conversion
let machin = parseFloat(truc);
console.log(machin); // Affiche le nombre à virgule flottante
//Convertir en nombre entier en utilisant parseInt() :

// Chaîne de caractères
let trucBis = "42";
// Utilisation de parseInt() pour la conversion
let machinBis = parseInt(trucBis);

console.log(machinBis); // Affiche le nombre entier
//Les fonctions parseFloat() et parseInt() analysent la chaîne de caractères en un nombre.
//parseFloat() renvoie un nombre à virgule flottante,
//tandis que parseInt() renvoie un nombre entier.
//Si la chaîne de caractères ne peut pas être convertie en nombre, elles renvoient NaN(Not - a - Number).

Créer chaine multi-lignes :
--------------------------

//Pour créer une chaîne de caractères sur plusieurs lignes en JavaScript, 
//vous pouvez utiliser la syntaxe des gabarits de chaînes (template literals) avec des backticks ( ). Voici un exemple :

// Utilisation des gabarits de chaînes pour créer une chaîne sur plusieurs lignes
let chaineMultiligne = `
Ceci est une chaîne de caractères
sur plusieurs lignes.
Elle peut contenir du texte
et des sauts de ligne facilement.`;
console.log(chaineMultiligne);

//En utilisant les backticks (`) pour délimiter la chaîne, vous pouvez insérer des sauts de ligne directement
//dans la chaîne sans avoir à utiliser des caractères d'échappement.
//Cela rend la création de chaînes sur plusieurs lignes beaucoup plus lisible et pratique.

Ajouter objet dans une liste préexistante avec push :
----------------------------------------------------


//Pour ajouter un dictionnaire (objet) comme élément à une liste en JavaScript, 
//vous pouvez simplement utiliser la méthode push().Assurez - vous que votre liste contient déjà au moins deux éléments 
//de types différents, puis ajoutez le dictionnaire comme suit:


// Liste initiale avec deux éléments de types différents
let maListe = [1, 'Bonjour'];

// Dictionnaire à ajouter
let monDictionnaire = { nom: 'John', age: 30 };

// Ajout du dictionnaire à la liste
maListe.push(monDictionnaire);

console.log(maListe); // La liste avec le dictionnaire ajouté
//Dans cet exemple, nous avons une liste initiale maListe contenant un nombre et une chaîne de caractères.
//Ensuite, nous ajoutons un dictionnaire monDictionnaire à cette liste en utilisant la méthode push().
//Après l'exécution de ce code, maListe contiendra trois éléments, dont le dernier sera le dictionnaire.

Ajouter liste valeur :
---------------------

//Pour ajouter une liste comme valeur dans un dictionnaire (objet) en JavaScript, 
//vous pouvez simplement attribuer cette liste à une nouvelle clé dans le dictionnaire.Assurez - 
//vous que votre dictionnaire contient déjà au moins deux autres paires clé - valeur, puis ajoutez la nouvelle paire clé - valeur comme suit:


// Dictionnaire initial avec deux paires clé-valeur
let newDictionnaire = {
    nom: 'John',
    age: 30
};

// Liste à ajouter comme valeur dans le dictionnaire
let newListe = [1, 2, 3];

// Ajout de la liste comme valeur dans le dictionnaire
newDictionnaire.newListe = newListe;

console.log(newDictionnaire); // Le dictionnaire avec la liste ajoutée
//Dans cet exemple, nous avons un dictionnaire monDictionnaire avec deux paires clé-valeur existantes
//(nom et age). Nous ajoutons ensuite une nouvelle paire clé - valeur en attribuant la liste maListe
//à la clé maListe du dictionnaire.Après l'exécution de ce code, monDictionnaire contiendra trois paires clé-valeur, la dernière étant la liste.

Taille d'une chaine :
--------------------

//Énoncé: Déterminez la longueur d'une chaîne de caractères.
//Contrainte: Utilisez une propriété de chaîne de caractères pour cela.

//Pour déterminer la longueur (le nombre de caractères) d'une chaîne de caractères en JavaScript, 
//vous pouvez utiliser la propriété length de la chaîne.Voici comment faire cela:


// Chaîne de caractères
let oldChaine = "Bonjour, c'est un exemple.";

// Utilisation de la propriété length pour obtenir la longueur
let longueur = oldChaine.length;

console.log("La longueur de la chaîne est : " + longueur);
//La propriété length renvoie le nombre de caractères dans la chaîne, y compris les espaces et les caractères spéciaux.
//Dans cet exemple, longueur contiendra la longueur de la chaîne maChaine, et cela sera affiché dans la console.

Majuscules et Minuscules toUpperCase | toLowerCase :
---------------------------------------------------

//Pour convertir une chaîne de caractères en majuscules et ensuite en minuscules en utilisant des méthodes de chaîne de caractères en JavaScript, 
//vous pouvez utiliser les méthodes toUpperCase() pour la conversion en majuscules et toLowerCase() pour la conversion en minuscules.Voici comment faire:


// Chaîne de caractères
let Chaine = "Exemple de Conversion";

// Conversion en majuscules
let enMajuscules = Chaine.toUpperCase();

// Conversion en minuscules
let enMinuscules = Chaine.toLowerCase();

console.log("En majuscules : " + enMajuscules);
console.log("En minuscules : " + enMinuscules);
//Dans cet exemple, nous utilisons toUpperCase() pour convertir la chaîne en majuscules et toLowerCase()
//pour convertir la chaîne en minuscules.Les résultats sont stockés dans les variables enMajuscules et enMinuscules,
//respectivement, puis affichés dans la console.

Remplacement dans une chaine replace :
-------------------------------------

//Pour remplacer un mot dans une chaîne de caractères en utilisant une méthode de chaîne de caractères en JavaScript,
// vous pouvez utiliser la méthode replace().Voici comment vous pouvez le faire:


// Chaîne de caractères
let maChaine = "Le chat est mignon. Le chat est joueur.";

// Mot à remplacer
let motAReplace = "chat";

// Nouveau mot
let nouveauMot = "chien";

// Utilisation de replace() pour effectuer le remplacement
let nouvelleChaine = maChaine.replace(motAReplace, nouveauMot);

console.log(nouvelleChaine);
//Dans cet exemple, nous utilisons la méthode replace() sur la chaîne maChaine pour remplacer toutes les occurrences du mot
//"chat" par "chien".Le résultat est stocké dans la variable nouvelleChaine et affiché dans la console.

//Notez que la méthode replace() ne modifie pas la chaîne d'origine mais renvoie une nouvelle chaîne avec les remplacements effectués.
// Si vous souhaitez effectuer le remplacement de manière globale(pour toutes les occurrences),
//utilisez une expression régulière avec le drapeau g comme ceci: maChaine.replace(/chat/g, "chien");.
//g pour général où global?

Extraire des élèments de chaîne :
--------------------------------

//Pour afficher les 5 premiers caractères et les 5 derniers caractères d'une chaîne de caractères en JavaScript 
//en utilisant des méthodes ou des propriétés de chaîne, vous pouvez faire ce qui suit:


// Chaîne de caractères
let maPhrase = "Exemple de chaîne de caractères à manipuler";

// Les 5 premiers caractères
let premiersCaracteres = maPhrase.slice(0, 5);

// Les 5 derniers caractères
let derniersCaracteres = maPhrase.slice(-5);

console.log("Les 5 premiers caractères : " + premiersCaracteres);
console.log("Les 5 derniers caractères : " + derniersCaracteres);
//Dans cet exemple, nous utilisons la méthode slice() pour extraire les 5 premiers caractères de la chaîne
//en spécifiant les indices de début et de fin(0 et 5), puis nous utilisons - 5 comme indice pour extraire
//les 5 derniers caractères de la chaîne.Les résultats sont stockés dans les variables premiersCaracteres et derniersCaracteres,
//respectivement, puis affichés dans la console.


Opération en chaine parseFloat | parseInt :
-----------------------------------------

//Pour effectuer une opération arithmétique avec deux nombres stockés sous forme de chaînes en JavaScript, 
//vous devez d'abord les convertir en nombres. Vous pouvez utiliser la fonction parseFloat() ou parseInt() 
//pour cela, en fonction de vos besoins(décimal ou entier).Voici un exemple avec parseFloat() pour effectuer une addition:


// Nombres stockés sous forme de chaînes
let nombre1 = "5.5";
let nombre2 = "3.2";

// Conversion des chaînes en nombres à virgule flottante
let nombre1EnNombre = parseFloat(nombre1);
let nombre2EnNombre = parseFloat(nombre2);

// Effectuer l'opération arithmétique (addition)
let resultat = nombre1EnNombre + nombre2EnNombre;

console.log("Résultat de l'addition : " + resultat);
//Dans cet exemple, nous utilisons parseFloat() pour convertir les chaînes nombre1 et nombre2 en nombres à virgule flottante.
//Ensuite, nous effectuons l'opération d'addition sur ces nombres et stockons le résultat dans la variable resultat.
//Le résultat est affiché dans la console.

//Vous pouvez également utiliser parseInt() si vous souhaitez effectuer des opérations avec des nombres entiers
//en convertissant les chaînes en nombres entiers.





<script src="src/script.js"></script>//pour ajouter un script JavaScript juste avant la fermante de body//

var nom = ['BENS']
console.log(nom)
var prénom = [' Hayete']
console.log(nom + prénom)
var age = 54
console.log(age)
var age1 = 5
console.log(age + age1)

(1) ["BENS"]
BENS Hayete
54
59
---------------------------------------------
|côté serveur : node.js où tri.js pour la 3D|
---------------------------------------------

-Une ligne de code est une instruction et le point virgule permet de dire à l'instructeur que l'instruction est terminée
et qu'il peut passer à l'instruction suivante.
-Un bloc d'instruction est limité par une accolade ouvrante et une fermante.
-L'eensemble entre ce bloc d'accolade font partie d'une instruction.


###Déclarer une variable (c'est donner une valeur)
------------------------

-Une variable est une case mémoire.

Il y a deux sortes de variables celles qui peuvent changer : let et var,
et celle qui ne change pas : const.

let alias = "Hayete"; //notez que l'on met des guillemets pour les string//
let price = 10;
let marque; //ici elle est indefined//
const myconst= 3; //elle sera toujours 3 quoiqu'il arrive//
let pricetwo = 23.

price * pricetwo / myconst;

ATTENTION : ON NE PEUT PAS DONNER DEUX FOIS LE MEME NOM A UNE VARIABLE.
-----------------------------------------------------------------------

DE MEME QU'ON NE PEUT PAS COMMENCER PAR UN CHIFFRE AU MILIEU OU A LA FIN C'EST POSSIBLE.
---------------------------------------------------------------------------------------

IL VAUT ECRIRE LES VARIABLES EN ANGLAIS.
---------------------------------------

EVITER D'AVOIR DES NOMS DE VARIABLES TROP LONG, ILS DOIVENT ETRE INTUITIFS ET DECRIRE CE QU'ILS CONTIENNENT.
------------------------------------------------------------------------------------------------------------

ATTENTION A LA CASSE; JS EST SENSIBLE A LA CASSE! Utilisez le camelcase.
------------------------------------------------------------------------

NE PAS UTILISEZ LES MOTS CLES DE JS POUR NOMMER LES VARIABLES.
-------------------------------------------------------------



##FONCTION
----------

Une fonction est une instruction effectuant une tâche où calculant une valeur, une fonction peut retourner des données où non.
Pour utiliser une fonction, il est nécessaire de l'avoir défini et déclarer pour pouvoir l'utiliser.

Entre les parenthèses nous y assignerons un où des arguments pour que la fonction puisse fonctionner correctement, mais cela n'est pas obligatoire.
Ces variables ne seront pas accessibles en dehors de cette fonction.


``Javascript
function multiplyBy(nb, nb2){
    //instructions
    return//dans le cas où l'on voudrait obtenir une réponse(ce qui n'est pas toujours obligatoire) le résultat, console.log, bouléan, etc...//
}
multiplyBy()
Le fait d'ouvrir des parenthèses cela s'appelle 'invoquer'.
Entre les parenthèse les données sont appellées 'paramétres'.

mutiplyBy(nb,nb2);

Pour le stocker dans une variable : 
let produit = multiplyBy(nb:23, nb2:9);
Pour l'afficher :
console.log('produit:', produit);

Nous pouvons obtenir plusieurs résultats dans le même console.log :
console.log(mutiplyBy(nb:48, nb2:59),mutplyBy(nb:21, nb2:14)multiplyBy(nb:12, nb2:25)); 

Exemple:
-------

function multiplyBy(nb3, nb4){
    consolelog('produit:'nb3 * nb4)
}
multiplyBy(nb3:1, nb4:6);
multiplyBy(nb3:2, nb4:7);
multiplyBy(nb3:3, nb4:8);
multiplyBy(nb3:4, nb4:9);
multiplyBy(nb3:5, nb4:10);


Pour vérifier une valeur:

function checkValue(value){
   console.log(value === 30);
}
checkValue(value:30);//retournera true
checkValue(value:33);//retournera false