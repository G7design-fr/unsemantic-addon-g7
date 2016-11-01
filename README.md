# Unsemantic addon g7 v1.0.1

Class CSS pour facilité le l'intégration responsive avec unsemantic

Cette class vous permettra de faciliter l'intégration responsive avec Unsemantic car elle vous permets de gérer des priorités de mise en forme et positionnement de blocs dans la même logique que Unsemantic pour définir sur quel affichage appliquer ces propriétés:

Par exemple en autre les possibilités de unsemantic qui gère les grilles par palier de 5% et le display block ou none cela l'affichage.
Vous pourrez définir si un element du dom est en block, inline ou inline bloc, l'alignement du texte, le float, le text-transform...
Une autre fonctionnement qui m'est très pratique est la gestion de l'espacement suivant l'affichage. Quand on passe au format mobile les éléments se chevauche et on souhaite parfois les aérer un peu. Avec cette Addon vous aurez 1800 classes d'espacement suivant l'affichage.
ex : <div class="space-10 mobile-space-30"></div> (un espace de 10px dans toute les configurations avec un espace de 30px pour l'affichage mobile)

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

# Utilisation

Ajoutez une ou plusieurs classes à votre élément du DOM 

Ex : 


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

Description :

Dans une grille Unsemantic on crée 2 colonnes en version Desktop et Tablet, 1 colonne en version mobile

  Desktop :
    - 2 colonnes
    - On affiche une bulle info en block
    - On dit défini une largeur maximum de 100% à l'image
    - On ne crée pas d'espace sous l'image
    - On appel le texte de la colonne de droite en justifié
    
  Tablet :
    - 2 colonnes
    - On affiche une bulle info en inline-block
    - On dit défini une largeur maximum de 100% à l'image
    - On ne crée pas d'espace sous l'image
    - On appel le texte de la colonne de droite en justifié
 
   Mobile :
    - 1 colonne, 2 lignes
    - On cache la bulle info
    - On dit défini une largeur maximum de 100% à l'image
    - On crée espace de 20 pixeils sous l'image
    - On appel le texte de la colonne de droite aligné a gauche
    

