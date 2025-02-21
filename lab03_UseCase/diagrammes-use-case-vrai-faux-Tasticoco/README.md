# Use case diagramme
![usecase](uml/usecase.png)
## Vrai ou faux
Etant donné le diagramme de cas d’utilisation ci-dessus, les assertions suivantes sont-elles vraies ou fausses ? 
- Une commande ordinaire est enregistrée par le vendeur
> VRAI: La commande ordinaire hérite de l'include de la commande.
- Une commande hors catalogue entraine un contrôle financier
> FAUX: Elle peut le faire mais ce ne sera pas garanti car la vérification `extends` l'enregistrement de la commande.
- Un client peut effectuer une commande hors catalogue
> VRAI: Le client peut atteindre a commande hors catalogue à travers son accès à l'étape parent `Effectuer une commande`.
- Le manager peut vérifier la commande sans effectuer de contrôle financier
> FAUX: La vérification de la commande `includes` le contrôle financier donc il sera appelé à toute vérification.
- Un client privilégié peut effectuer une commande ordinaire
> VRAI: Car il hérite du client ordinaire qui peut atteindre la commande ordinaire par son accès à l'étape parent `Effectuer une commande`.

## Modifier le diagramme 
Comment modifier ce diagramme pour qu’un client non privilégié ne puisse effectuer de commande hors catalogue ?

> On associe le client à la commande ordinaire et on enlève son association à `Effectuer une commande`. Grâce à ce changement le client privilégié pourra accéder à la commande ordinaire par son héritage de client et le client ne pourra plus qu'accéder à la commande ordinaire par sa seule association avec la commande ordinaire.

