[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/hQGWoEnc)
# Diagrammes de classe - HAUTE ÉCOLE

## Objectifs
- Prendre en main plantuml pour la création des diagrammes UML.
- Mettre en pratique vos connaissances dans la modélisation de domaine (diagrammes de classe).
  
## Commencer avec plantuml
- Pour un démarrage rapide, vous pouvez installer le plugin plantuml pour votre IDE.
  https://plantuml.com/fr/starting
- Explorez comment créer des diagrammes de classe avec plantuml :
  https://plantuml.com/fr/class-diagram

## Consignes
Réalisez le diagramme de classe (de domaine) correspondant à la description suivante.
### Haute école
On considère l’organisation d’une haute école pour laquelle on à 3 types de membres: Professeurs, assistants et étudiants. On connait le nom et prénom de tous les membres. Par ailleurs, on sait à quelle filière les étudiants appartiennent et dans quel institut les professeurs travaillent.
<br><br>
Chaque professeur est expert dans un certain nombre de disciplines et l’école désirant assurer une certaine redondance, il y a au moins 2 professeurs experts dans chaque discipline. Par ailleurs, chaque assistant doit indiquer son niveau de compétence dans chacune des disciplines proposées. Ce niveau varie entre 1 (faible) et 4 (expert)
<br><br>
Chaque cours est donné par un professeur et encadré par au plus 3 assistants. Par soucis pédagogique, un cours ne peut couvrir de matière que d’une seule discipline. Par soucis financier, l’école n’ouvre pas de cours pour moins de 5 étudiants. 

_**PS.**_ Procéder en étapes, et enrichir votre diagramme progressivement :
- Identifier les classes conceptuelles.
- Identifier les associations et les classes d’associations.
- Identifier les attributs.
- Identifier les cardinalités.

## Rendu
- Créer votre diagramme en utilisant plantuml dans un fichier séparé.
- Faire un commit et un push vers votre repo.
- Rendre le lien de voter repo dans le devoir Teams.