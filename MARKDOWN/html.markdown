#HTML
=====

- <br>--revient à la ligne
- <hr>--fait un trait de ligne
- atribut--ajoute des propriétés spéciales à la balise (entre les guillemets = valeur) 
- tag = balise
- //html select tag//
- Pour les commentaires en html Crtl/

###Créer une deuxième page html et la relier 
-----------------------------------------

- Il est important de garder le nom : index.html car l'interpreteur saura que c'est la première page!

- Créer une page html classique, index.html
puis y mettre une ancre dans le body

```html
<a href="pageDeux">
<h1>page 2</h1> </a>(le titre est cliquable mais ne mène nulle part à ce stade!)

créer une deuxième page html par exemple pageDeux.html

<a href="index.html">
<h1>page 1</h1>
</a>
```

- Le titre page 1 est cliquable et nous dirigera vers la pageDeux.
NB. Nous pouvons mettre un texte entre les balises a (ex: cliquez ici, suivant, précedent, etc...)
sans mettre de titre.

Chemin relatif et absolu
------------------------

 Le chemin absolu commence à la racine du système de fichiers, tandis que le chemin relatif part du répertoire courant.
 
Formulaire
----------

<form>
Prénom: <input type="text" name="Prénom"><br> (le Prénom sera écrit à l'éx,térieur du champ, pas ce qu'on écrira!)
Nom: <input type="text" name="Nom"><br>
Téléphone: <input type="number" name="Téléphone"><br>
Email: <input type="email" name="Email"><br>
Date de naissance: <input type="date" name="Date de naissance"><br> 
Mot de passe: <input type="password" minlingth="8" required name="Mot de passe"><br>
Genre:<br> 
<input type="radio" name="genre" value="Homme">Homme<br>
<input type="radio" name="genre" value="Femme">Femme<br>
Nous leur avons donné un name pour les regroupés et en selectionné un seul.

Animaux:<br>
<input type="checkbox" name="animal" value="Chien">Chien<br>
<input type="heckbox" name="animal" value="Chat">Chat<br>
Ici les cases à cocher sont carré et on peut tous les cocher.
Plats:<br>

Aprés "select" nous pouvons mettre "multiple", afin d'ajouter d'autre'(s) attribut(s).<br>
L'attribut "name" permet d'afficher dans l'html chaque champ.<br>
Dans l'exemple ci-dessus, j'ai rajouté name pour chaque input afin de l'afficher dans mon IDE.<br>
Il faudra copier/coller les informations qui sont dans la barre de recherche. Et le coller dans l'IDE.<br>
? Pour signifier qu'il y a des informations aprés.<br>
Attributs/valeurs<br> 
%40 = encodage spéciale = @ /Tout comme (? où &)


<select name="plats">
<option value="chakchouka">chakchouka</option>
<option value="pizza">pizza</option>
<option value="couscous">couscous</option>
</select>
Affiche menu déroulant
</form>

Nous pouvons ajouté la propriété "required" pour obliger la personne à remplir obligatoirement le champ,
"required" n'a pas besoin de valeur car il est spéciale et doit rendre comme valeur "true".
Envoyer: <input type="submit" value="s'inscrire"><br> (Si on ne donne pas de nom il aura automatiquement le nom envoyer)
<input type="reset"><br> Il affichera réinitialiser au cas où il y aurau une(des) erreur(s) !


Méthodes GET POST
-----------------

De base, lorsqu'on envoie un formulaire, c'est la méthode GET qui est par défault.<br>
Nous utiliserons POST pour l'envoyer directement au back-end. 



