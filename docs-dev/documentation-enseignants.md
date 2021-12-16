# Insérer une image dans les consignes ou les sujets

Lorsque l'on souhaite insérer une image dans les consignes ou les sujets, il n'est pas possible de le faire comment on le ferait avec un document Word, LibreOffice ou Google Doc. Les images ne peuvent pas être incorporées depuis un emplacement présent sur la machine de l'utilisateur. Elles doivent être placées sur internet et accessibles depuis une adresse directe.

## Syntaxe
Soit une image présente à l'adresse suivante : https://www.exemple.com/images/monimage.png.

Pour insérer cette image, deux syntaxes sont possibles :

* `![](https://www.exemple.com/images/monimage.png)`\
Le texte entre crochets est optionnel, il ne sert qu'à décrire l'image si jamais l'image ne s'affiche pas. Avec cette syntaxe, il n'est pas possible de modifier la taille l'image. Elle s'affichera dans sa taille originale.

* `<img src="https://www.exemple.com/images/monimage.png" width="50" />`\
Avec cette syntaxe, on peut spécifier la largeur de l'image grâce à la déclaration <kbd>width</kbd>. Le chiffre indiqué est exprimé en pixels. A la place de <kbd>width</kbd>, il est possible d'utiliser <kbd>height</kbd> pour définir la hauteur de l'image. Il est aussi possible d'utiliser <kbd>width</kbd> et <kbd>height</kbd> en même temps, mais attention à ne pas déformer l'image. Faites des essais.

