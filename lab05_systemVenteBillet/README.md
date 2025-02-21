# Système de vente de billets de concert

## Consignes

Dans ce cas d'étude, vous allez travailler sur la modélisation d'un système de vente de billets pour des concerts en utilisant UML.

Vous devez réaliser
- un diagramme de cas d'utilisation (use case diagram),
- un diagramme de classes (class diagram) et
- un diagramme de séquences (sequence diagram)
pour représenter les principales fonctionnalités et interactions du système.

Une fois les diagrammes réalisés, veuillez les soumettre pour évaluation et feedback.
<br>
**Labo noté**, travail à réaliser en groupe, un rendu par groupe.
<br>
Pour rendre le travail, il faut soumettre un lien vers le hash du commit de votre repository.

Les diagrammes doivent être cohérent, non-ambigus et non-redondants.

## Contexte

Une entreprise spécialisée dans l'organisation de concerts souhaite développer un système en ligne
pour faciliter la vente de billets.

Ce système doit permettre aux utilisateurs d'accéder à des informations sur les concerts, de
commander des billets de concert pour des places numérotées, de payer des billets en ligne, et de
recevoir des billets par email.

De plus, le système doit permettre aux administrateurs de gérer des salles, des places, des concerts,
des artistes, et le tarif appliqué aux places de concert.

## Exigences fonctionnelles
1. Les utilisateurs doivent pouvoir créer un compte et se connecter au système à l’aide
d’un email et d’un mot de passe. Durant le processus de connexion, le système peut
décider de passer par un 2FA (Authentification multi facteurs). La création des nouveaux
comptes ainsi que les connexions au système sont gérées par un serveur
d’authentification.
2. Les utilisateurs doivent pouvoir consulter la liste des concerts disponibles et leurs
informations (date, heure, salle, artistes, nombre de places disponibles, et à quel tarif).
3. Les utilisateurs doivent pouvoir sélectionner un concert et commander un ou plusieurs
billets. La réservation se fait en trois étapes : vérifier la disponibilité des places, payer les
billets et envoyer une confirmation à l’utilisateur. Chaque billet a un code unique qui est
vérifié à l’entrée du concert.
4. Les utilisateurs doivent pouvoir payer leurs billets en utilisant l’un des moyens suivants :
carte bancaire ou PayPal. Le paiement est traité à l’aide du système de la banque.
5. Les utilisateurs doivent recevoir une confirmation par e-mail avec les détails de leur
réservation et leurs billets électroniques. La confirmation n'est envoyée à l'utilisateur que si le paiement a été effectué avec succès.
1. En plus de ce qu’un utilisateur peut faire, un administrateur doit pouvoir modifier les
informations liées aux concerts (ajout, suppression, tarif, ..).

## Remarques complémentaires
- La programmation d’un concert comprend un ou plusieurs artistes
- Une commande contient un ou plusieurs billets
- Un billet concerne une place numérotée lors d’un concert
- Une salle de concert est composée de places numérotées
- Le tarif d’une place peut varier selon le concert

## Travail à réaliser

1. Réalisez un diagramme de cas d'utilisation (use case diagram) pour représenter les
principales fonctionnalités et interactions entre les acteurs (utilisateurs et administrateurs)
et le système.
2. Réalisez un diagramme de classes (class diagram) pour modéliser les entités du système
(concert, billet, artiste, tarif, moyen de paiement, messagerie, etc.), leurs relations, et leurs
attributs. Il n’y a pas besoin d’ajouter les méthodes à cette étape.
3. Réalisez un diagramme de séquences (sequence diagram) pour décrire les interactions entre
les objets lors de la finalisation de la commande d’un utilisateur. Le diagramme doit illustrer
le calcul du montant total de la commande, le paiement de la commande à l’aide d’un
moyen de paiement, et l’envoi de la commande à l’utilisateur par email. 
Afin de faire le lien avec le diagramme de classe réalisé à l'étape 2, ajouter les méthodes utilisées dans le diagramme
de séquence à votre diagramme de classe. Seules ces méthodes doivent figurer sur le diagramme de
classe.
