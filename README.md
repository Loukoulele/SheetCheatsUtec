![Badge Language](https://img.shields.io/badge/Language-HTML-blue) ![Badge Status](https://img.shields.io/badge/Status-En%20Cours-yellow)
<p align="center" style="text-align: center;">
<img src="./HTML5_Logo.svg" alt="HTML5 Logo" height="256" /><br>
</p>
<h1 class="text-blue" style="color: #ea8853; font-weight: 400">Cheatsheet HTML5</h1>
<hr>

## Information de réalisation

Ce mémoire est basé sur des recherche et fondé aussi sur nos connaissances personnels et est réalisé pour l'école d'UTEC d'Émerainville.

Théme : HTML5

Date de rendu : 16/03/2020

Mémoire réalisé par Ilan B., Maxime C., Jordan L.

## Introduction HTML

Le "HyperText Markup Language" est un langage de balisage conçu pour représenter des pages webs qui est apparu en 1989. Il a été conç principalement pour rediriger vers des liens externes, aujourd'hui ce langage est utilisé pour
réalisé des site internet. En 1997 la mis à jour vers html4 à vue le jour, et nous sommes actuellement sur HTML5 depuis son apparition en 2008.

## HTML History

* 1989	Tim Berners-Lee invented www
* 1991	Tim Berners-Lee invented HTML
* 1993	Dave Raggett drafted HTML+
* 1995	HTML Working Group defined HTML 2.0
* 1997	W3C Recommendation: HTML 3.2
* 1999	W3C Recommendation: HTML 4.01
* 2000	W3C Recommendation: XHTML 1.0
* 2008	WHATWG HTML5 First Public Draft
* 2012	WHATWG HTML5 Living Standard
* 2014	W3C Recommendation: HTML5
* 2016	W3C Candidate Recommendation: HTML 5.1
* 2017	W3C Recommendation: HTML5.1 2nd Edition
* 2017	W3C Recommendation: HTML5.2

Pour commencer nous allons voir les différentes balises et évolution de ce langage et en fin de parti nous parlerons des nouvelles updates de HTML 5.1 et HTML 5.2.

Aujourd'hui W3C reconnait W3C comme une norme en langage d'affichage orienté web.

## Qu'est ce que HTML5 ?

HTML5 n'est pas qu'une simple mis à jour suivant HTML4, c'est un langage complet qui a pour but de simplifier les développeurs à utiliser un maximum d'outil utile sur les sites web. HTML4 se contenté au bon affichage sur la page web, alors qu'aujourd'hui il se focalise essentiellement sur les applications WEB et ces intéractivité.

## HTML5 Guidelines

HTML5 est la dernière version du standard HTML. Cette nouvelle version contient de nouveaux éléments, attributs, comportements et un large panel de technologie qui permettent de construire des sites et applications performants et divers.

* **Sémantique** : permets de décrire plus en détail votre contenu.
* **Connectivité** : permets de communiquer avec les serveurs d'une façon nouvelle et innovante.
* **Hors ligne et stockage** : permets de stocker des données du côté du client en locale et faire des opérations hors ligne efficacement.
* **Multimédia** : fournit une nouvelle façon de gérer les objets multimédias.
* **Graphiques 2D/3D et effets** : propose de nouvelles façons de présenter.
* **Performance et integration** : fournit une grande vitesse d'optimisation et une meilleure utilisation du matériel.
* **Accès aux appareils** : permets l'utilisation d'une variété d'appareils et support récent de la géolocalisation.
* **Habillé** : permets de créer des styles attirants et petillants.

## Modèle basique

```HTML
<!DOCTYPE html>
<html lang="en" dir="ltr">

  <head>
    <meta charset="utf-8">
    <title>Example</title>
  </head>

  <body>
    <p>Hello world!</p>
  </body>

</html>
```

# Qu'est ce que le Doctype ?

Un Doctype est une ligne de code servant a indiquer le Type de votre document. Le Doctype précise les normes définis que vous allez donc utilisé dans ce document. Lorsque vous codez une page web en HTML, vous devez définir son Doctype.

La ligne de code contenant le Doctype s’insère en tout début de page. Vous pouvez la placez à la première ligne de votre document HTML si vous souhaitez. Le Doctype doit toujours se situer avant la balise <HTML>.

Pour un développeur, le Doctype lui sert à valider ses pages suivant les normes W3C choisis. Mais son principal but est d’indiquer aux navigateur comment interpréter le document – ou page web.

L’arrivé des navigateurs modernes à tous bouleversé. Ils ne portent que peu d’intérêt à cette balises mise à part le cas particuliers des quirks modes. HTML 5 allant dans le sens de ses évolutions, le doctype fût donc simplifié au maximum.

# Pourquoi faut-il respecter les normes du W3C ?

Bien que le strict respect des normes W3C n’est pas d’effet particulier sur le référencement, il parait préférable de les suivre au maximum. Néanmoins, certaines erreurs peuvent nuire grandement à l’indexation de votre site. Par exemple, ne pas mettre de balise \<title> entre les balises \<head> ne gênera pas vos visiteurs mais affectera votre positionnement sur Google.

Les normes ont été créer pour éviter que tout le monde se disperse et chacun y gagne en compatibilité.

Une page web respectant les standards réduira son risque d’incompatibilité entre les différents navigateur et la plateforme sur laquelle il tourne (téléphone mobile, grand écran, tablette ….).

# Se tenir à jour sur le support des navigateurs

Les navigateurs sont sujets à une évolution constante de leurs composants, ce qui rend difficile de se renseigner sur le support des fonctionnalités HTML5 de notre navigateur. Certains sites permettent de suivre ces informations comme [caniuse](https://caniuse.com/) ou [w3school](https://www.w3schools.com/tags/default.asp)

### Structure d'un document en HTML 5

```HTML
<!DOCTYPE html>
<html>
 <head></head>
 <body>Corps de la page</body>
</html>
```

# Exemple de nouvel balise dans HTML5 :

* **video** : Celui-ci ressemble à la balise img, on déclace plusieurs chemin d'une vidéo au cas ou si le navigateur ne prend pas en compte l'extension.

```HTML
<!DOCTYPE html>
<html lang="en" dir="ltr">

  <head>
    <meta charset="utf-8">
    <title>Example</title>
  </head>

  <body>
    <video controls width="250">

    <source src="/media/examples/flower.webm" type="video/webm">

    <source src="/media/examples/flower.mp4" type="video/mp4">
      Sorry, your browser doesn't support embedded videos.
    </video>
  </body>

</html>
```

* **meter** : L'élément meter représente une valeur scalaire dans un intervalle donné ou une valeur fractionnaire.

```HTML
<!DOCTYPE html>
<html lang="en" dir="ltr">

  <head>
    <meta charset="utf-8">
    <title>Example</title>
  </head>

  <body>
    <label for="fuel">Fuel level:</label>

    <meter id="fuel"
           min="0" max="100"
           low="33" high="66" optimum="80"
           value="50">
        at 50/100
    </meter>
  </body>

</html>
```

* **progress** : L'élément HTML progress indique l'état de complétion d'une tâche et est généralement représenté par une barre de progression.

```HTML
<!DOCTYPE html>
<html lang="en" dir="ltr">

  <head>
    <meta charset="utf-8">
    <title>Example</title>
  </head>

  <body>
    <label for="file">File progress:</label>

    <progress id="file" max="100" value="70"> 70% </progress>
  </body>

</html>
```

* **output** : Le formulaire qui suit fournit un curseur dont la valeur peut aller de 0 à 100 ainsi qu'un élément \<input> dans lequel on peut saisir un deuxième nombre. Les deux nombres sont additionnés et le résultat est affiché dans l'élément output et est actualisé lorsqu'une des deux valeurs est modifiée.

```HTML
<!DOCTYPE html>
<html lang="en" dir="ltr">

  <head>
    <meta charset="utf-8">
    <title>Example</title>
  </head>

  <body>
    <form oninput="result.value=parseInt(a.value)+parseInt(b.value)">
        <input type="range" name="b" value="50" /> +
        <input type="number" name="a" value="10" /> =
        <output name="result">60</output>
    </form>
  </body>

</html>
```

## Guide

### Lien CSS

On ne peut parler de HTML5 sans évoquer CSS3 qui vont de paire. Pour plus de performance on va importer les feuilles dans le head. Cela permet de mettre du 'design' sur la page web, le css permettra d'appliquer des couleurs, de la mise en forme etc ...

On peut lier du css avec la balise style (peu recommandable) :
```HTML
<head>
  <style>
    body {
      background-color: aliceblue;
    }

    p {
      font-size: 2em;
      color: red;
    }
  </style>
</head>
```

On peut aussi lier des fichiers css externes en indiquant leur chemin :
```HTML
<head>
  <link href="/css/main.css" rel="stylesheet"> <!-- Absolu -->
  <link href="css/main.css" rel="stylesheet"> <!-- Relative -->
</head>
```

On peut lier des fichiers css par lien CDN :
```HTML
<head>
  <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" rel="stylesheet">
</head>
```

Voici quelques nouveautés qu'apporte CSS3 :

* Border-radius : permet d'ajouter une courbe à la bordure d'une balise.
* Box-shadow : permet d'ajouter une ombre sur certaines balises.
* Text-shadow : permet d'ajouter une ombre à du texte.
* Gradients : permet de créer des dégradés de couleurs de façon lineaire ou radiale.

### Lien Javascript

Pour plus de performance on va importer les scripts à la fin du body.

On peut lier du javascript avec la balise script (peu recommandable) :
```HTML
<body>
  <p>Hello World!</p>

  <script type="text/javascript">
    window.alert('hello world');
  </script>
</body>
```

On peut aussi lier des fichiers js externes en indiquant leur chemin :
```HTML
<body>
  <p>Hello World!</p>

  <script type="text/javascript" src="js/main.js"></script> <!-- relative -->
  <script type="text/javascript" src="/js/main.js"></script> <!-- absolu -->
</body>
```

On peut lier des fichers js par lien CDN :
```HTML
<body>
  <p>Hello World!</p>

  <script src="https://code.jquery.com/jquery-3.4.1.min.js"
    integrity="sha256-CSXorXvZcTkaix6Yvo6HppcZGetbYMGWSFlBw8HfCJo="
    crossorigin="anonymous"></script>
</body>
```

### De nouvelles balises HTML5

<**nav**> | Balise pouvant servir à créer une barre de navigation :
```HTML
<nav>
  <a href="#">home</a>
  <a href="#">hello</a>
  <a href="#">world</a>
  <a href="#">!</a>
</nav>
```

<**footer**> | Balise pouvant servir à créer un bas de page récurrent ou non :
```HTML
<footer>
  <span>Copyright @ UTEC</span>
</footer>
```

<**progress**> | Balise pouvant servir à créer une barre de progression (souvent couplé avec du javascript) :
```HTML
<progress value="25" max="100">25%</progress>
```

<**source**> <**video**> <**audio**> | Balise pouvant servir à afficher des vidéos ou de l'audio sur la page :
```HTML
<video controls width="250" height="200" muted>
  <source src="/media/examples/flower.webm" type="video/webm">
  <source src="/media/examples/flower.mp4" type="video/mp4">
  This browser does not support the HTML5 video element.
</video>
```

La nouvelle balise vidéo permet aussi de gérer le controleur et le comportement de la vidéo (Si la vidéo doit se lancer automatiquement lorsque la page est chargé)
Attention le support de la vidéo peut varié en fonction des formats (mkv, webm, mp4....) et du navigateur (chrome, firefox, opera...)

```HTML
<audio controls src="/media/examples/t-rex-roar.mp3">
  Your browser does not support the audio element.
</audio>
```

De même que pour la balise video, la compatibilité avec le navigateur sera en fonction du format de l'audio (mp3, ogg, flac...).

Des librairies Javascript permettent notamment de faciliter l'utilisation de ces balises et d'en compléter le fonctionnement :

* Popcorn.js
* Html5Media

<**canvas**> | Balise permettant de dessiner, traiter des images et pouvant même créer un jeu complet.

C'est une forte alternative pour eviter l'integration de script flash ou encore java pour réaliser des taches que ces deux languages permettaient de faire plus simplement.

```HTML
<canvas id="myCanvas" width="600" height="600">
  Votre navigateur ne supporte pas le canvas !
</canvas>
```

#### 2D

Pour dessiner avec un canvas on va utiliser la liaison avec l'API de dessin 2D via Javascript :

```HTML
<script>
  var draw = document.getElementById('myCanvas');
  var shape = draw.getContext('2d');
  shape.fillStyle = "blue";
  shape.fillRect(200, 200, 500, 500);
</script>
```

Les formes primitives du canvas se limitent d'une part à des fonctions de la famille des rectangles :

* **fillRect(x, y, l, h)** | un rectangle plein
* **strokerect(x, y, l, h)** | le contour d'un rectangle
* **clearRect(x, y, l, h)** | Rectangle vide

D'autre part le canvas permet une liberté de traçage d'un chemin pour créer ses propres formes.

* **beginPath()** | permet de commencer le traçage.
* **moveTo(x, y)** | permet de se deplacer dans l'espace sans dessiner.
* **lineTo(x, y)** | permet de tracer une ligne de l'emplacement jusqu'au point indiqué.
* **closePath()** | permet de finir le traçage.

Bien d'autre fonctions sont disponible pour laisser libre cours à l'imagination.

#### 3D

Le passage vers la balise canvas à permit d'introduire le support de webGL. weebGL est un API javascript conçue la création en 3D. webGL est aujourd'hui supporter par la plupart des navigateurs

```JavaScript
function main() {
  const canvas = document.querySelector("#myCanvas");
  const gl = canvas.getContext("webgl");

  if (gl === null) {
    alert("Unable to initialize WebGL. Your browser or machine may not support it.");
    return;
  }

  gl.clearColor(0.0, 0.0, 0.0, 1.0);
  gl.clear(gl.COLOR_BUFFER_BIT);
}

window.onload = main;
```

### Création des stockages distincts

Avant HTML5, les données applicatives était stockées dans les cookies inclues dans chaque requête serveur. L'introduction d'HTML5 introduit de ce fait un nouveau type de stockage et celui-ci plus sécurisé. On peut alors stocker une grande quantité d'informations sans impacter les performances du site web. Par rapport aux cookies la limite de stockage est bien plus conséquente (au moins 5mb) et les données ne sont jamais envoyées vers un serveur. Ces stockages web sont délimité par origine (nom de domaine), ce qui veut dire que toute page venant de la même origine qu'une autre aura accès à la donnée.

```javascript
// Store
localStorage.setItem("lastname", "Smith");

// Retrieve
document.getElementById("result").innerHTML = localStorage.getItem("lastname");

//clear
localStorage.removeItem("lastname");
```

Il existe deux types de stockage :

* localStorage : C'est un stockage qui est permanent il sera uniquement supprimé lors de la desinstallation du navigateur ou de l'effacement forcé des cookies.
* sessionStorage : Il est similaire au localStorage à l'exception qu'il garde la donnée que pour une session. Donc les données sont effacés lorsque l'utilisateur ferme l'onglet specifc à la session.

Ces stockages sont de type clé/valeur, ce qui se rapproche fortement du comportement du language JSON avec des fonctions spécifique à la manipulation de la données.  

### Les déconnexions inattendues

HTML5 propose aux utilisateurs pocesseur de faible connexion la possibilité de consulter un site web même en étant hors ligne. Cela joue avec un système de cache mis en place par le navigateur.

```YAML
# html5.appcache
CACHE MANIFEST
# Version 1
CACHE:
# index.html est caché par défaut (contient le lien vers le MANIFEST)
index.html
style.css
img/html5.png
NETWORK:
FALLBACK:
```

```HTML
<!-- index.html -->
<!DOCTYPE html>
<html manifest="html5.appcache">
...
</html>
```

### Geolocalisation

L'introduction de la geolocalisation dans le navigateur a permis un avancé majeur dans le traitement et la mise a disposition d'information selon la localisation. Ce traitement est géré par l'API geolocalisation HTML5 en javascript.

```javascript
if (navigator.geolocation) {
  navigator.geolocation.getCurrentPosition(function(position) {
    pos  = "Latitude : " + position.coords.latitude  + "<br/>";
    pos += "Longitude: " + position.coords.longitude + "<br/>";
    pos += "Altitude : " + position.coords.altitude  + "<br/>";
    document.getElementById("myPosition").innerHTML = pos;
  },
  function(position) {
    document.getElementById("myPosition").innerHTML = "Impossible de vous localiser" ;
  });
} else {
  document.getElementById("myPosition").innerHTML = "Service non disponible" ;
}
```

## Syntaxe de projet

### Structure des balises head et body

Un espace entre html et head et pas d'indentation sur le head. De même entre le head et le body et le body et html indentation sur les fils des deux blocks :

```HTML
<html>

<head>
  <meta charset="utf-8">
</head>

<body>
  <p>hello world</p>
</body>

</html>
```

### Syntaxe balises auto-fermantes :

Les balises se ferment avec la syntaxe html5 c'est à dire sans le slash ("/") de fermeture
```HTML
<meta charset="utf-8">
```

ou

```HTML
<img src="https://image.com/myimage" />
```

### HTML attribut lang

Ne pas oublier l'attribut lang à placer sur la balise HTML :
```HTML
<html lang="fr">
```

Il aide entre autre au référencement par exemple des robots Google qui permettent d'indexer le contenu en fonction de la langue de la géololisation.

### Balise Title

Ne pas omettre la balise title :
```HTML
<title>Hello World</title>
```

### Balise Meta

Il faut absolument preciser au navigateur de quelle façon il doit décoder le texte du site :
```HTML
<meta charset="utf-8">
```

### Aider le référencement Google

Eviter de placer la même balise description dans deux pages de votre site.
Evitez de lister des mots-clés en guise de description de page, vous serez alors considérés comme des spammeurs. Il faut que votre description soit le développement de votre titre et le résumé de votre page.

```HTML
<meta name="description" content="description de la page">
```

# Qu'est ce qu'un moteur de template moderne ?

Il existe différent type de moteur de template qui permet de compilé des modéeles en php par exemple pour optimisé simplement la page web et évite la surcharge.
Exemple : Twig, Mustache, Handlebars, doT, pug etc ...

### HTML/PHP classique :

```HTML
<body>
  <?php
  if (isset($_POST)) {
      $stmt = $db->prepare("INSERT INTO users (:username, :email)");
      $stmt->execute([
          ':username' => $_POST['username'],
          ':email' => $_POST['email']
      ]);
  } else {
      echo "<table><tr><th>Username</th><th>Email</th></tr>";

      $stmt = $db->prepare("SELECT * FROM users");
      $stmt->execute();

      while ($r = $stmt->fetch(PDO::FETCH_ASSOC)) {
          echo "<tr><td>$r['user_name']</td><td>$r['email']</td></tr>";
      }

      echo "</table>"
  }
  ?>
</body>
```

### Moteur de template (Twig) :

```HTML
<body>
  <table>
      <tr>
          <th>Username</th>
          <th>Email</th>
      </tr>

      {% for user in users %}
          <tr>
              <td>{{user.user_name}}</td>
              <td>{{user.email}}</td>
          </tr>
      {% endfor %}
  </table>
</body>
```

### Liste exhaustive de moteur :

| Nom                                                 | Language   |
| ---                                                 | ---        |
| [Pugjs](https://pugjs.org/api/getting-started.html) | Javascript |
| [Jinja](https://jinja.palletsprojects.com/en/2.11.x/) | Python   |
| [EJS](https://ejs.co/)                              | Javascript |

Nous pouvons voir la simplicité et une grosse réduction de code coté front. Cela permet aussi d'alléger et d'augmenter la sécurité de l'application web.

# API HTML5

Comme nous l'avons vu précédement, HTML5 ce veux plus optimisé pour les applications web, c'est pour cela qu'il permet d'utiliser 8 nouvelles API qui permettront de créer de nouvelles applications et qui peuvent être utilisées ensemble avec de nouveaux éléments introduits pour les applications dont :

* Une API de dessin 2D utilisé avec la nouvelle balise canvas.
* Une API pour jouer des vidéos et des sons/musiques utilisé avec les nouvelles balises video et audio.
* Une API utilisée pour les applications hors-lignes.
* Une API d'édition en combinaison avec le nouvel attribut contenteditable.
* Une API de drag and drop en combinaison avec l'attribut draggable.
* Une API qui permet l'accès à l'historique et permet aux pages d'en ajouter pour prévenir les problèmes de bouton retour-en-arrière.

# Connexion et distribution P2P

HTML 5 se voit doté de la capacité de réaliser des connexions entre utilisateurs PeerToPeerConnection(), et également grâce aux websocket. Grâce à la création de nouvelles balises, on voit que l'on va pouvoir améliorer le référencement de son site grâce notamment à aside, nav, header et footer...

## HTML5.1 2e édition

Elle a commencé a être développer en décembre 2012 et a était validé en novembre 2016.

* **Picture et srcset** : Pour commencer l'ajout du picture et srcset. Cela permet d'optimiser la bande passante du serveur car il permet de charger les images en fonction d'une taille d'écran (responsivité)

```HTML
<picture>
  <source media="(max-width: 480px)"
            srcset="http://monurl.fr/small.jpg">
  <source media="(max-width: 640px)"
            srcset="http://monurl.fr/medium.jpg">
  <source media="(max-width: 1024px)"
            srcset="http://monurl.fr/large.jpg">
  <img src="http://monurl.fr/large.jpg" alt="Faon">
</picture>
```

Celle ci est relativement similaire à la méthode de la balise vidéo qui permet de gérer les différentes extensions en fonction du navigateur, néanmoins ici il permet de gérer les tailles d'écrans et si aucune n'est compatible alors retourner une image par défaut.

* **Details et summary** : Ceci permet de ne plus utilisé de javascript pour déplier un contenu (collapse en bootstrap).

```HTML
<details>
  Ceci est un texte.
</details>
<details open>
  <summary>
    Introduction
  </summary>
  Angular 2 est un framework JavaScript développé par Google. Son code a été complètement revu par rapport à Angular 1, blablabla...
</details>
```
On peut apercevoir que HTML veux simplifié l'utilisation de balise sans forcement appliqué du css ou du js pour utilisé quelque chose de courant dans le web.

* **Menu contextuel** : Ceci permet d'ajouter des fonctionalités au menu de votre navigateur. Il est possible d'associer un élement de votre page à un menu personnalisé.

```HTML
<p contextmenu="custom-menu">
  Faites un clic droit sur ce paragraphe pour ouvrir le menu personnalisé, Firefox only :(
</p>

<menu type="context" id="custom-menu">
  <menuitem type="checkbox" checked="true">Je suis une checkbox</menuitem>
  <menuitem type="command" icon="https://www.grafikart.fr/images/logo.png" onclick="window.open('https://www.grafikart.fr/q/php+tutoriel', 'shareWindow');">Rechercher sur le site</menuitem>
</menu>
```

* **Nouveaux types : week, month, datetime-local** : De nouveau type d'input pour les dates, semaines, mois ou un systeme de calendrier.

```HTML
<input type="week"> permet de sélectionner une semaine spécifique sous forme de : semaine / année.
<input type="month"> permet de sélectionner un mois spécifique sous forme de : mois / année.
<input type="datetime-local"> permet de sélectionner une date spécifique sous forme de : jour / mois / année / heure / minute.
```

* **Amélioration des API HTML5** : il y a d'autres changements comme l'amélioration de l'API requestAnimationFrame pour faire des animations plus efficaces, la suppression de l'attribue multiple pour les inputs de type range, l'ajout de la méthode reportValidity() qui retourne immédiatement à l'affichage d'une page si un formulaire est valide ou non, etc.

Nous pouvons voir de nouvelles améliorations liés à cette mise-à-jour. Ce n'est effectivement pas une update majeur mais elle a son lot de spécifité qui permet d'améliorer nettement la qualité de développement pour les développeur.

### HTML 5.3
La technologie HTML5 en est à sa version 5.2, le W3C travaille actuellement sur une version 5.3 qui apportera de nouvelles fonctionnalités permettant d’aider les auteurs d’applications Web. Il a rendu publique le travail concernant la version 5.3.
Sa consultation est libre sur le site : ww.w3.org/TR/html53/

### Extensibilité

En termes d’extensibilité, avec HTML 5.3 les auteurs peuvent :
* Créer des éléments personnalisés afin de créer de nouveaux comportements
* Utiliser l’attribut « class » pour annoter des éléments. Il s’agit d’une des fonctionnalités primaires du CSS
* Utiliser <meta name=““ content=““> pour inclure des métadonnées à l’échelle de la page
* Annoter des liens avec des significations spécifiques avec rel=““
* Manipuler des scripts en ligne ou côté serveur à l’aide de <script type=““>
* Étendre les API grâce au mécanisme de prototypage de JavaScript

Il sera également possible de capitaliser automatiquement avec l’autocappitalize attribute. Cette fonctionnalité permettra de :
* Mettre automatiquement en majuscule toutes les lettres des champs de saisie
* Mettre le premier caractère de chaque mot en majuscule
* Mettre en majuscule le premier caractère de chaque phrase

Une autre mesure, les auteurs doivent déterminer si la ou les nouvelles fonctionnalités seront accessibles à des utilisateurs atteints d’handicap et si ces fonctionnalités peuvent dégrader la confidentialité et la sécurité des utilisateurs. Il est également important de prendre en compte l’internationalisation des utilisateurs. Il est impératif de prendre en compte ces considérations pour de meilleures pratiques de l’HTML.

## Balisage de présentation

La version 5.3 axe ses modifications sur l’HTML sémantique. C’est-à-dire l’utilisation du balisage de présentation. Le sémantisme vise à renforcer le sens des informations contenues dans les pages web. Grâce à de nouvelles balises sémantiques, les moteurs de recherches et autres logiciels pourront mieux évaluer l’importance du contenu d’un site web.
Une grande partie des fonctionnalités de présentation des versions précédentes de HTML ne sont plus supportées, le balisage de présentation présente plusieurs problèmes :
* Moins d’accessibilité, par exemple pour présenter le balisage de présentation, des auteurs utilisaient ARIA (Applications Internet Riches et Accessibles) qui est un ensemble d’attribut permettant de rendre le contenu et les applications web accessibles. Cependant la plupart des widgets ont été intégrés au sein d’HTML5 et il est préférable aujourd’hui d’utiliser un balisage sémantique.
* Coût de maintenance élevé, il est plus simple de maintenir un site intégrant des balises sémantiques appropriées.
* Taille des documents, l’usage de balise de présentation peut être redondant et ainsi augmenter la taille des documents.

C’est pourquoi le balisage de présentation est supprimé dans la version 5.3. HTML 4.0 avait abandonné le balisage de présentation il y a quelques années. Cependant il reste encore 2 fonctionnalités de balisage de présentation style attribute et <style> element
Nous pouvons remarquer que dans cette nouvelle version 5.3, certains éléments de balisage de présentation ont été redéfinies :
* <b>
* <i> exemple : <i> deviendra en balise sémantique <em> qui indiquera une mise en valeur
* <hr>
* <s>
* <small>
* <u>


### HTML5, interactif et innovant

HTML5 est également utilisé dans des domaines tels que l’univers du jeu vidéo, l’animation vidéo. HTML est considéré comme un « accélérateur » du web permettant aux développeurs de créer des expériences innovantes.
Le but est de ne pas laisser l’utilisateur visiter passivement le site web, grâce aux technologies comme Three.js, WebGL, Javascript, HTML5 intègre des composants modernes, 3D, des ressources permettant de rendre le site plus dynamique, intéractif également.
Nous pouvons citer le site : fiscalkombat.fr qui sur un site web permet de jouer à un jeu vidéo

![img]("Assets/example1.png")

En ce qui concerne le domaine vidéo nous pouvons citer le site : video.bobdylan.com
Le site en lui-même est une vidéo, nous pouvons voir que l’HTML5 permet de transformer un simple curseur en une télécommande interactive et d’immerger l’utilisateur sur le site internet.

![img]("Assets/bobdylan.png")

HTML permet de donner un côté immersif, interactif aux sites web. Les site web deviennent de réels acteurs du digital et permettent de véhiculer des messages, des histoires, des ambiances.

### Cyber-sécurité

La cyber-sécurité est au cœur des nouvelles mesures de la version 5.3.
Première mesure : Scriptage intersite (XSS)
Les données doivent être validées avant utilisation, si une étape de validation n’est pas gérée par l’auteur, un attaquant peut effectuer différents types d’attaques. XSS appelée Cross-Site Scripting est une faille de sécurité importante car elle permet l’injection de code HTML ou JavaScript.
Pour s’en protéger, il existe la fonction « htmlspecialchars() qui permet de filtrer les symboles spéciaux comme <, &, “ en les remplaçant par leur équivalent HTML :
Exemple : Le symbole & deviendra &amp.
Deuxième mesure : CSRF (Cross-Site Requuest Forgery)
Cette attaque consiste à usurper l’identité d’un utilisateur de confiance et permet d’envoyer des commandes, instructions sur un site web.
Pour se prémunir de ces attaques, les auteurs doivent inclure des jetons appelés « tokens » dans les formulaires HTML.

### Interopérabilité

Définition d’interopérabilité : Notion transversale permettant à divers outils/produits/systèmes/services de communiquer entre eux.

Grâce à l’HTML et son interopérabilité il est possible de visualiser des pages web sur différent device. Car rappelons que l’HTML n’est pas fait pour spécifier l’apparence d’un site web et ses pages, mais plutôt pour mettre l’accent sur l’importante et le sens du contenu.
Son haut degré d’interopérabilité justifie la baisse des coûts fournisseurs de contenus car une version de chaque document sert des besoins différents.

C’est pourquoi que lorsque l’on développe une application web, l’auteur doit s’assurer de l’interopérabilité de son application, qu’elle peut être implémenté par la plupart des différents implémentateurs.

Prenons un exemple de non-interopérabilité actuelle, du fait qu’Internet Exlorer ne prenne pas en charge certaines normes Web supplémentaires (HTML5), certaines de ses pages WEB continuent d’utiliser des balises HTML non standardisées et qui nuit à l’interopérabilité des navigateurs.

Cette interopérabilité de l’HTML n’est pas seulement visible sur le plan hardware, mais également sur le plan de navigateurs web que nous allons aborder juste après.

## HTML5, un standard

Actuellement, HTML5 est utilisé par les navigateurs les plus courants (Google Chrome, Firefox, Opera, Safari).
Voici un tableau récapitulatif des navigateurs supportant plus ou moins bien HTML5.

| Navigateur                                                 | Version   | Efficacité |
| ---                                                 | ---        |  --- |
| Google Chrome | 80.0 | Excellente |
| Opéra | 66.0   | Excellente |
| Mozilla Firefox                              | 73.0 | Bonne |
| Safari                              | 13.0 | Bonne |
| Internet Explorer                              | 10 | Mauvaise |

**Rappelons la définition d’un standard** : Un standard est un élément de référence, une norme de fabrication.
Le consortium W3C est l’organisme chargé de mettre en œuvre les standards du web. Son but est de promouvoir la compatibilité des technologies du web dont HTML5.

Le W3C se repose du quatre principes :

* La simplicité
* La modularité
* La compatibilité
* L’extensibilité

Ces principes nous les retrouvons dans le langage HTML5. Le langage HTML est un élément de référence dans le monde du web puisqu’il est un langage de balise conçu pour représenter les pages web. C’est donc un standard du web.

HTML5 vise à enrichir le langage web pour faciliter la création de clients web riches tout en maintenant une rétrocompatibilité optimale avec l’existant.
Définition rétrocompatibilité : Aptitute d’un matériel/servie à prendre en charge le même ensemble d’instructions qu’un système plus ancien.

## Code propre avec HTML5

Il est toujours agréable pour un développeur d’avoir un code propre. Mais qu’est-ce qu’un code propre ? En plusieurs points c’est :
* Un code agréable à lire  
* Facile à comprendre
* Structuré, organisé
* Noms de fichiers clairs
* Sans erreurs

Avoir un code HTML propre comporte plusieurs avantages :
* Tout d’abord c’est réutilisable par tous, donc une facilité d’amélioration, de continuité
* Permet d’avoir un web standardisé avec des règles uniformisées
* Simplifie et réduits les coûts de maintenance

Comment se construit un code HTML propre ? Par sa structure qui se compose de :
* L’indentation du code
* Les noms des fonctions et des variables
* Les accolades
* Les appels de fichiers

Ce code propre impactera énormément le référencement SEO appelé également le référencement naturel d’un site internet, les moteurs de recherche trouveront plus facilement un site internet bien structuré, avec un code lisible, clair.
Pour vérifier si notre code HTML est propre, l’organisme W3C a mis au point un outil en ligne permettant de vérifier si notre site internet est conforme aux normes W3C : validator.w3c.org

## HTML5 les fonctionnalités retirées

HTML5 continue de s'améliorer que ce soit dans le sens d'ajout de nouvelles fonctionnalités comme des balises, des créations de nouvelles APIs etc..., mais aussi dans le sens de revoir ce qui est existant et de définir si l'utilité persiste ou non.

Voila une liste exhaustive des fonctionnalités supprimés dans cette version 5 de HTML :

Les éléments ci-dessous ne sont plus valides dans HTML5 car la fonctionnalité apportée par ceux-ci sont aujourd'hui mieux géré par le moteur de style `CSS`.

* <**basefont**> : permet de définir les paramètres de la font basique utilisée.
* <**big**> : permet de rendre le texte plus grand.
* <**center**> : permet de centrer le texte.
* <**font**> : permet de surcharger la font utilisée par le texte.
* <**strike**> : permet de barré le texte.
* <**tt**> : permet de donner un style particulier au texte.

Les éléments ci-dessous ne sont plus acceptés par HTML5 car ils causent des problèmes d'utilisation et d'accessibilité.

* <**frame**> : permet de définir un affichage de fenêtre avec un fichier appelé.
* <**frameset**> : permet de définir une liste de frame.
* <**noframes**> : permet d'avertir l'utilisateur que son navigateur ne supporte pas les frames.

Les éléments ci-dessous ont été supprimé à cause de leur sous utilisation.

* <**acronym**> : permet de donner plus d'informations sur un acronyme. Il est remplacé par le tag <**abbr**>
* <**applet**> : permet d'importer des script java dans une page web. Il est remplacé par <**embed**> ou <**object**>
* <**isindex**> : permet de faire une requête sur les pages d'un site web et lister les pages qui corréspondent.
* <**dir**> : permet de créer une liste non ordonée. Il est remplacé" par le tag <**ul**>

Les différent tags sont encore accessible mais ne seront, pour la plupart, pas supporté par le navigateur.

![img]("Assets/htmlchecker.png")

# Utilité aujourd’hui d’utiliser HTML5

L’engouement provoqué par HTML5 avec la communauté web permet de dire qu’aujourd’hui, HTML est un standard du web. Du fait que la majorité des site internet sont construits avec l’HTML, le CSS et le JavaScript, l’HTML5 regroupe cet ensemble de technologie. Dans le futur il sera indispensable pour tout navigateurs d’intégrer toutes les fonctionnalités de l’HTML5.

Les spécifications de l’HTML5 version 5.3 ne sont à l’heure actuelle pas encore terminées, elles viennent de commencer car il est long de pouvoir recenser, et penser aux nouvelles fonctionnalités de demain tout en répondant au maximum aux besoins des utilisateurs.

Aujourd’hui la simplicité d’utilisation de l’HTML5 permet à n’importe qui se former rapidement et de pouvoir se lancer rapidement dans la construction de son propre site internet sans de grosses connaissances informatiques.
L’HTML5 n’est pas une révolution, mais une évolution logique des technologies ayant construit le web.

On le voit aujourd’hui les plus grands sites intègrent HTML5 (Apple, Google, Gmail, YouTube).

Comme dit précédemment, HTML5 de par son succès, devient un réel standard du web.

Nous pouvons voir au début de cette image < !doctype html> qui est simplifié au maximum, HTML5 est donc dans la simplicité.

![img]("Assets/html.png")

<hr>

## Source (pour nous) :  
Detail + history :

* https://openclassrooms.com/fr/courses/1916641-dynamisez-vos-sites-web-avec-javascript/1921707-quest-ce-que-le-html5
* https://fr.wikipedia.org/wiki/Hypertext_Markup_Language
* https://www.w3schools.com/html/html5_intro.asp
Doctype :
* http://41mag.fr/un-doctype-simplifie-en-html-5.html
Nouvel balise HTML5 :
* https://developer.mozilla.org/fr/docs/Web/HTML/Element/video
* https://developer.mozilla.org/fr/docs/Web/HTML/Element/output
* https://jaetheme.com/balises-html5/
* https://www.aurone.com/les-nouveaut%C3%A9s-apport%C3%A9es-par-html-5
Template engine :
* https://twig.symfony.com/
* https://learn.userfrosting.com/templating-with-twig/overview
API HTML 5 :
* https://www.programmation-facile.com/api-javascript-html5-utiliser-sites-web/
HTML 5.1 :
* https://www.w3.org/TR/html51/
* https://www.grafikart.fr/blog/w3C-html-5-1
HTML 5.2 :
* https://www.w3.org/TR/html52/

https://www.millenium.org/news/156787.html
https://blog.equancy.com/le-futur-de-la-publicite-en-ligne-cest-html5-et-cest-maintenant/
https://www.w3.org/TR/html53/
https://developer.mozilla.org/fr/docs/Accessibilit%C3%A9/ARIA
https://www.justegeek.fr/les-navigateurs-internet-et-le-html5/
http://prof.bpesquet.fr/cours/html5-en-bref/
https://validator.w3.org/nu/?doc=https%3A%2F%2Fwww.switech.fr%2F
https://www.agenceici.com/le-blog/article/les-sites-web-se-doivent-de-respecter-la-norme-w3c-73
https://verekia.com/html5/introduction-html5/#part4-3
