#CSS
====
 
 - Aprés avoir lié le css au html(<link rel="stylesheet" href="index.css">)où (link rel="stylesheet" href="./index.css")(on peut aussi ajouter quel type de css) exemple: text/css<br>

 - Nous avons la possibilité d'ajouter un nouveau css, pour une nouvelle page. (link rel"stylesheet" href="style2.css")<br>

sélecteur {
    propriété: valeur;
}
 
 /*--commentaires en css--*/

 sélecteur simple:<br>

```css
body {
    /*télégarger une image*/
    baground-image: url("préciser le nom de l'image");
    baground-size: cover;
}
 h2 {
    color: green;
    text-align: center;
    border: 5px solid purple;
    cursor: pointer;
 }

p {
    color: purple;
}
li {
    list-style: none; 
    /*pour retirer les points*/
}
.boxmode1 {
    display: inline-bloc;
    /*--Pour se mettre les uns à côté des autres et non naturelemment les uns au-dessous des autres--*/
    border: 5px solid green;
    padding: 22px;
    /*--les valeurs commencent par haut, droite, bas, gauche, si les meusures sont différentes, nous donneront 4 valeurs, sinon une où deux.--*/
    /*--marge intérieure--*/
    marging: 30px;
    /*--marge extérieure, pour les valeurs pareil que les padding, ATTENTION: CSS donne par défaut un marging, pour l'enlever, on utilisera: style: non--*/
}
```

- Nous pouvons aussi injecté du css directement dans le html.Ex: <header style="baground-color: blue";color: yellow;>

- Et dans le head: <style>
li {
    bagroundcolor: pink;
}
</style>

Séparation des préoccupation
----------------------------

Une façon elegante de dire: chacun son taf dans le projet! (Pour faciliter l'organisation avec une équipe de développeurs.)

!important = permet d'imposer ses règles qui prime sur tout le reste.


Les unités de mesures
---------------------

Les unités sont données en px(pixels).
em est par exemple dans un texte multiplier par 5 la valeur px(pour décorer où mettre en valeur un mot, une phrase, etc...).

Flexbox
-------

```css
.container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
} 
 
 h1 {
    border-bottom: 2px dotted pink;
    /*--dotted = pointillé--*/
    box-shadow: 5px 5px 5px grey;
    /*--l'exemple du dessous c'est dans les cas où un des navigateurs ne supporte pas notre code car nouveau--*/
    -moz-box-shadow: 5px 5px 5px grey;
    /*--mozilla--*/
    -ms-box-shadow: 5px 5px 5px grey;
    /*--?--*/
    -webkit-box-shadow: 5px 5px 5px grey;
    /*--?--*/
    -o-box-shadow: 5px 5px 5px grey;
    /*--opéra--*/

 }
 img {
    transition: all 1s;
    /*--nous voulons donner ue transition--*/
 }
 img: hover {
    tansform: scale (1.1);
    /*--quand on survole l'image elle s'agrandit légèrement--*/
 }
 ```

