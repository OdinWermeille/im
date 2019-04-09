# Frontend MVC avec Backbone et Bootsrap

  

## Mise en place

Le *design pattern* mise en place dans les TP précédents nous aide à avoir une architecture de code propre. Backbone.js et Handlebars nous permettent de simplifier notre architecture de code, la gestion des événements ainsi que la modification du DOM.   Il nous reste toutefois le travail complexe de l'ergonomie applicative *responsive*. Afin d'éviter un long travail en HTML et CSS, il existe de multiples *frameworks* nous offrant les composants de base pour la réalisation d'une interface Web *responsive*. Nous allons dans ce TP utiliser le plus utiliser d'entre eux: [Boostrap](https://getbootstrap.com/). Commencez donc par l'installer (ainsi que sa dépendance à *popper.js*) avec *npm*. Profitez aussi d'installer [Backbone.LocalStorage](https://github.com/jeromegn/Backbone.localStorage) qui permettra de faire une persistance des données Backbone directement dans le LocalStorage.

```bash
npm install bootstrap popper.js backbone.localstorage--save
```
Il nous vous restera plus qu'à l'importer dans votre code pour en bénéficier:

```js
import 'bootstrap';
import 'bootstrap/dist/css/bootstrap.min.css';
import {LocalStorage} from 'backbone.localstorage';
```
En plus de s'initier à un *framework* de design d'interface Web, ce TP à comme objectif de faire réviser les différentes pièces du design pattern MVC. Vous devez réaliser un « embryon » d’application pour un shop en ligne proposant des périphériques informatiques de type souris, claviers et casques audio uniquement. 

## Cahier des charges

L'application doit  afficher la liste des produits sur la page. Les produits seront définis par 4 champs: le modèle, la marque, le prix et le type (qui ne peut être que "mouse", "keyboard" et "headset"). L'utilisateur pourra naviguer entre les 3 types de produits grâce à 3 boutons de filtre. Il pourra aussi trier la liste affichée par prix croissant ou décroissant. 

L'utilisateur pourra ajouter un produit à son caddie d'achat. Pour des raisons de simplification, la quantité ne sera pas à gérer. Le produit sera alors simplement ajouté au caddie de l'utilisateur en un seul exemplaire.   L'utilisateur pourra visualiser son caddie en cliquant sur l'icone associée. La page du caddie affichera la liste des produits avec les prix ainsi que le prix total  actuel. Enfin, L'utilisateur pourra supprimer un produit de son caddie.

**Indications:** commencez par identifier les différents *Models* nécessaires. Modélise 




<!--stackedit_data:
eyJoaXN0b3J5IjpbLTcxMzcxNTk2MSwtMTk4NTAxMDc2Nyw5MT
Q4MDM5MDMsMTE4Mjg1NzU2OV19
-->