# Diagramme de classe

![Classes](uml/classes.png)

## Vrai ou faux

Etant donné le diagramme de domaine ci-dessus, les assertions suivantes sont-elles vraies ou fausses ? 
- Etudiant est une classe d’association
> FAUX: étudiant est une classe conceptuelle différemment de la classe "Cours"
- Un étudiant peut participer à autant de cours qu’il veut
> VRAI: la cardinalité "*" nous l'indique
- Plusieurs professeurs peuvent enseigner la même discipline
> FAUX: la cardinalité "1" nous l'indique
- Un professeur peut enseigner plusieurs disciplines
> VRAI: la cardinalité "*" de l'association nous l'indique
- Un cours peut être enseigner à 2 étudiants
> FAUX: la cardinalité nous indique qu'il nous faut au minimum 5 étudiants
- Un cours peut être enseigner à 20 étudiants 
> VRAI: elle peut être enseignée jusqu'à 30 étudiants

## Question ouverte

Représentez la même association avec la notation UML « petit losange » 

- Quelles informations perd-on par rapport au diagramme ci-dessus ? 
> On perd la cardinalité sur la discipline et les potentiels attributs de Cours