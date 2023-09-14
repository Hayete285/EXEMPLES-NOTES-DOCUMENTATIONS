#JAVASCRIPT
==============

Déclarer une variable :
----------------------

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
console.log(fruits[0],fruits[2])

bonjour il y a des pommes dans le rayon fruit
//à noter nous avons ajouter un s car pomme était au singulier//
pomme
bananne

<script src="src/script.js"></script>//pour ajouter un script JavaScript juste avant la fermante de body//