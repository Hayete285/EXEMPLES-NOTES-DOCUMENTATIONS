#NODE.JS ET EXPRESS
===================


Pour lier Node.js à HTML et créer des applications web dynamiques,
je peux utiliser un framework web tel que Express.js. 
Voici les étapes pour lier Node.js à HTML en utilisant Express.js :

###Installez Node.js et Express.js : 
-----------------------------------

Si vous ne l'avez pas déjà fait, 
installez Node.js sur votre système. 
Express.js est un framework pour Node.js, 
vous pouvez l'installer via npm 
(le gestionnaire de paquets de Node.js) 
en exécutant la commande suivante dans votre terminal :

npm install express --save
Cela installera Express.js et ajoutera une entrée dans le fichier package.json de votre projet.

###Créez un serveur web Express :
-------------------------------

 Vous devez créer un serveur web en utilisant Express.js.
  Voici un exemple de code pour créer un serveur web simple :

````javascript
Copy code
const express = require('express');
const app = express();
const port = 3000;

// Servez des fichiers statiques (comme des fichiers HTML, CSS, JavaScript, etc.)
app.use(express.static('public'));

// Définissez une route pour la page d'accueil
app.get('/', (req, res) => {
    res.sendFile(__dirname + '/public/index.html');
});

app.listen(port, () => {
    console.log(`Serveur en cours d'exécution sur le port ${port}`);
});
````
``
Dans cet exemple, nous créons un serveur Express qui écoute sur le port 3000. 
Nous utilisons express.static pour servir des fichiers statiques depuis le dossier "public", 
ce qui inclut les fichiers HTML.

###Créez votre fichier HTML :
---------------------------

 Créez un fichier HTML (par exemple, index.html) dans le dossier "public" 
 (ou tout autre dossier que vous avez spécifié dans express.static). 
 Vous pouvez ajouter du contenu HTML à ce fichier, 
 y compris des balises script pour inclure des scripts JavaScript si nécessaire.

###Créez des routes pour les pages HTML :
----------------------------------------

 Vous pouvez définir des routes Express pour gérer les demandes HTTP 
 et envoyer les fichiers HTML appropriés en réponse à ces demandes. 
 Dans l'exemple ci-dessus, 
 nous avons défini une route pour la page d'accueil ("/") qui envoie le fichier "index.html".

###Exécutez votre serveur Node.js : 
----------------------------------

Exécutez votre serveur Node.js en exécutant la commande suivante dans le terminal :

node server.js
Assurez-vous que "server.js" est le nom du fichier dans lequel vous avez placé le code du serveur Express.

####Accédez à votre application web : 
------------------------------------

Ouvrez un navigateur web et accédez à http://localhost:3000 
(ou le port que vous avez spécifié) pour voir votre application web en action.

En suivant ces étapes, vous avez réussi à lier Node.js à HTML à l'aide d'Express.js.
 Vous pouvez maintenant développer des applications web plus complexes en ajoutant des routes, 
 des contrôleurs et des fonctionnalités dynamiques en utilisant Node.js et Express.js.





