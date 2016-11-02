# Unsemantic addon g7 v1.0.1

Class CSS pour faciliter l'intégration responsive avec unsemantic

Cette class vous permettra de faciliter l'intégration responsive avec Unsemantic car elle gère des priorités de mise en forme et positionnement de blocs dans la même logique que Unsemantic pour définir sur quel affichage appliquer ces propriétés:

Par exemple les possibilités de Unsemantic qui gère initialement les grilles par palier de 5% ainsi que le display block ou none selon l'affichage (Desktop, Tablet, Mobile).
Vous pourrez définir si un élément du dom est en block, inline ou inline bloc, l'alignement du texte, le float, le text-transform...
Une autre fonctionnement qui m'est très pratique est la gestion de l'espacement suivant l'affichage. Quand on passe au format mobile les éléments se chevauchent et on souhaite parfois les aérer un peu. Avec cet Addon vous aurez 1800 classes d'espacement suivant l'affichage.
ex : 
```sh
<div class="space-10 mobile-space-30"></div> 
```
(un espace de 10px dans toute les configurations avec un espace de 30px pour l'affichage mobile)

Les propriétés :
Elles sont toutes défini initialement + affichage mobile, tablette, écran

- text-align:right;
- text-align:left;
- text-align:center;
- text-align:justify;
- white-space:nowrap;
- text-transform:lowercase;
- text-transform:uppercase;
- text-transform:capitalize;
- float:right!important;
- float:left!important;
- float:none!important;
- display:block!important;
- display:inline!important;
- display:inline-block!important;
- max-width:100%;
- max-width:none; 

Espacement :
Pour chaque affichage vous pourrez définir un espacement différent de la même façon de 0 à 449px de height;
Il y a 1800 classes pour 4 configuratios d'affichages :

- Mobile
- Tablette 
- Ecran
- Toutes les configurations (mais pas en priorité sur les autres types)


# Requires

Unsemantic CSS Framework
"Responsive CSS Class"
http://unsemantic.com

# Installation

Appeller la class css après Unsemantic

# Exemple

Ajoutez une ou plusieurs classes à votre élément du DOM 

Ex : 

```sh
<div class="grid-container grid-parent">

  <div class="grid-50 tablet-grid-50 mobile-grid-100">
  
    <div class="hide-on-mobile display-block tablet-display-inline-block">bulle info<div>
    <div class="maxw100">block image<div>
    <div class="space-none mobile-space-22">block image<div>
    
  </div>
  <div class="grid-50 tablet-grid-50 mobile-grid-100">
  
    <div class="text-justify mobile-text-center">block texte<div>
    
  </div>

</div>
```
##Description :

Dans une grille Unsemantic on crée 2 colonnes en version Desktop et Tablet, 1 colonne en version mobile

####Desktop :
- 2 colonnes
- On affiche une bulle info en block
- On dit défini une largeur maximum de 100% à l'image
- On ne crée pas d'espace sous l'image
- On appel le texte de la colonne de droite en justifié
    
####Tablet :
- 2 colonnes
- On affiche une bulle info en inline-block
- On dit défini une largeur maximum de 100% à l'image
- On ne crée pas d'espace sous l'image
- On appel le texte de la colonne de droite en justifié
 
####Mobile :
- 1 colonne, 2 lignes
- On cache la bulle info
- On dit défini une largeur maximum de 100% à l'image
- On crée espace de 20 pixeils sous l'image
- On appel le texte de la colonne de droite aligné a gauche

# Lexique des classes

##Utilisation des classes suivant d'affichage

Aucune diférence avec Unsemantic

```sh
<div class="mobile-... //Pour l'affichage Mobile (- de 768px)
<div class="tablet-... //Pour l'affichage Tablette (entre 769 et 1024px)
<div class="destkop-... //Pour l'affichage Ecran (+ de 1025px)
```

La différence est que toutes les classes sont appelées aussi sans les @medias query pour être appliqué dans toutes les configurations

Au lieu de 

```sh
<div class="mobile-display-block"></div>
```

il faudra appeller la classe 

```sh
<div class="display-block"></div>
```

(Les classes mobile-, tablet- et desktop- prennent le dessus sur une classe appellé sans query)

##Liste des classes

#### Textes

* .text-left
* .text-right
* .text-center
* .text-justify
* .text-nowrap
* .text-lowercase 
* .text-uppercase 
* .text-capitalize

#### Block/inline

* .pull-right
* .pull-left
* .pull-none
* .display-block 
* .display-inline
* .display-inline-block
* .maxw100 (max-width:100%;)
* .maxwnone (max-width:none;)

##Classes .Spaces

Les classes .space ont la même logique :


Tous les affichages (non prioritaire sur les Querys) :

* .space-0
* .space-none
* .space-1
* .space-2
* ...
* .space-449

Mobile :

* .mobile-space-0
* .mobile-space-none
* .mobile-space-1
* .mobile-space-2
* ...
* .mobile-space-449

Tablette :

* .tablet-space-0
* .tablet-space-none
* .tablet-space-1
* .tablet-space-2
* ...
* .tablet-space-449

Ecran :

* .desktop-space-0
* .desktop-space-none
* .desktop-space-1
* .desktop-space-2
* ...
* .desktop-space-449

    

