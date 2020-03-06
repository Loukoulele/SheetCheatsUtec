![Badge Language](https://img.shields.io/badge/Language-HTML-blue) ![Badge Status](https://img.shields.io/badge/Status-En%20Cours-yellow)
<p align="center" style="text-align: center;">
<img src="./HTML5_Logo.svg" alt="HTML5 Logo" height="256" />
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

## Qu'est ce que HTML5 ?

HTML5 n'est pas qu'une simple mis à jour suivant HTML4, c'est un langage complet qui a pour but de simplifier les développeurs à utiliser un maximum d'outil utile sur les sites web. HTML4 se contenté au bon affichage sur la page web, alors qu'aujourd'hui il se focalise essentiellement sur les applications WEB et ces intéractivité.

## HTML5 Cheatsheet

HTML5 est la dernière version du standard HTML. Cette nouvelle version contient de nouveaux éléments, attributs, comportements et un large panel de technologie qui permettent de construire des sites et applications performants et divers.

* **Sémantique** : permets de décrire plus en détail votre contenu.
* **Connectivité** : permets de communiquer avec les serveurs d'une façon nouvelle et innovante.
* **Hors ligne et stockage** : permets de stocker des données du côté du client en locale et faire des opérations hors ligne efficacement.
* **Multimédia** : fournit une nouvelle façon de gérer les objets multimédias.
* **Graphiques 2D/3D et effets** : propose de nouvelles façons de présenter.
* **Performance et integration** : fournit une grande vitesse d'optimisation et une meilleure utilisation du matériel.
* **Accès aux appareils** : permets l'utilisation d'une variété d'appareils.
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

Bien que le strict respect des normes W3C n’est pas d’effet particulier sur le référencement, il parait préférable de les suivre au maximum. Néanmoins, certaines erreurs peuvent nuire grandement à l’indexation de votre site. Par exemple, ne pas mettre de balise <title> entre les balises <head> ne gênera pas vos visiteurs mais affectera votre positionnement sur Google.

Les normes ont été créer pour éviter que tout le monde se disperse et chacun y gagne en compatibilité.

Une page web respectant les standards réduira son risque d’incompatibilité entre les différents navigateur et la plateforme sur laquelle il tourne (téléphone mobile, grand écran, tablette ….).

### Structure d'un document en HTML 5

```HTML
<!DOCTYPE html>
<html>
 <head></head>
 <body>Corps de la page</body>
</html>
```

# Exemple de nouvel balise dans HTML5 :

* **<video>** : Celui-ci ressemble à la balise <img>, on déclace plusieurs chemin d'une vidéo au cas ou si le navigateur ne prend pas en compte l'extension.

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

* **<meter>** : L'élément <meter> représente une valeur scalaire dans un intervalle donné ou une valeur fractionnaire.

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

* **<progress>** : L'élément HTML <progress> indique l'état de complétion d'une tâche et est généralement représenté par une barre de progression.

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

* **<output>** : Le formulaire qui suit fournit un curseur dont la valeur peut aller de 0 à 100 ainsi qu'un élément <input> dans lequel on peut saisir un deuxième nombre. Les deux nombres sont additionnés et le résultat est affiché dans l'élément <output> et est actualisé lorsqu'une des deux valeurs est modifiée.

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

Pour plus de performance on va importer les feuilles dans le head. Cela permet de mettre du 'design' sur la page web, le css permettra d'appliquer des couleurs, de la mise en forme etc ...

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

<**source**> <**video**> <**audio**> | Balise pouvant servir à afficher des vidéos ou de l'audio sur la page) :
```HTML
<video controls width="250" height="200" muted>
  <source src="/media/examples/flower.webm" type="video/webm">
  <source src="/media/examples/flower.mp4" type="video/mp4">
  This browser does not support the HTML5 video element.
</video>
```

```HTML
<audio controls src="/media/examples/t-rex-roar.mp3">
  Your browser does not support the audio element.
</audio>
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

### HTML attribut lang

Ne pas oublier l'attribut lang à placer sur la balise HTML :
```HTML
<html lang="fr">
```

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

Nous pouvons voir la simplicité et une grosse réduction de code coté front. Cela permet aussi d'alléger et d'augmenter la sécurité de l'application web.
