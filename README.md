[C#](https://exercism.org/tracks/csharp/concepts)
# Programmation Orientée Objet
La Programmation Orientée Objet (ou POO) est un paradigme (modèle) de programmation dans lequel les programmes sont écrits et structurés autour des objets.

![test](https://i.stack.imgur.com/nAtpl.png)
## Exemple
un exemple dans la vrai vie, une voiture est un objet, avec ses attributs (type, modèle, prix, couleurs, etc…) et ses méthodes (accélérer, ralentir, tourner, freiner, etc.).

![POO](car-poo.png).

# Principes de la POO
- **L’encapsulation** masque les détails d’implémentation d’une classe à d’autres objets.
- **L’héritage** est un moyen de former de nouvelles classes en utilisant des classes déjà définies.
- **Le polymorphisme** est le processus d’utilisation d’un opérateur ou d’une fonction de différentes manières pour différentes entrées de données.
- **L’abstraction** simplifie la réalité complexe en modélisant des classes appropriées au problème.
- **L'nterface** En termes simples, une interface est comme un contrat, où chaque membre ou composant inclus dans le corps doit suivre le contrat
# Une Class
Une classe est un plan de déclaration et de création d'objets.

# Un Objet
Un objet est une instance de classe qui permet aux programmeurs d'utiliser des variables et des méthodes à partir de l'intérieur de la classe.

# Les principes du Clean Code
- Un code aussi simple que possible : KISS (construire leur code de façon aussi simple que possible)
- Éviter les répétitions inutiles : DRY (chaque fonctionnalité doit avoir une seule et unique représentation).
- Supprimer ce qui est inutile : YAGNI
# Principe solide 
| S |  Responsabilité unique (Single responsibility principle)|  Une classe doit avoir une et une seule responsabilité|
|:--|:--|:--|
| O | Ouvert/fermé (Open/closed principle) | Une classe doit être ouverte à l'extension, mais fermée à la modification |
| L | Substitution de Liskov (Liskov Substitution Principle) | Une instance de type T doit pouvoir être remplacée par une instance de type G, tel que G sous-type de T, sans que cela modifie la cohérence du programme |
| I |Ségrégation des interfaces (Interface segregation principle)  |  Préférer plusieurs interfaces spécifiques pour chaque client plutôt qu'une seule interface générale|
| D | Inversion des dépendances (Dependency Inversion Principle) | Il faut dépendre des abstractions, pas des implémentations |

# Patrons de conception

 [Patrons de conception](https://refactoring.guru/fr/design-patterns/creational-patterns).

![p1](patron1.png).

![p2](patron2.png).

# Test 

| Type de test | définition | frameworks C# | frameworks Angular |
|:--|:--|:--|:--|
| Intégration | Consiste à tester comment certaines parties de l'application fonctionnent ensemble dans son ensemble (connexion de la BD) | xUnit | Karma et Jasmine |
| Unitaire | Les tests unitaires se concentrent sur une seule partie d'une application, généralement une seule classe ou fonction |  | Karma et Jasmine |
| E2E |  |  | Protractor to Cypress |

# async et await

Pour permettre à une méthode longue de retourner le trait immédiatement (ou en tout cas au plus vite), elle peut exécuter son code en créant un tâche (Task). Le mot clé await permet d’attendre la fin d’une telle tâche. Async permet de marquer une méthode qui fera usage de await.

## Fixons les choses

- Une méthode async ne peut retourner que void ou une Task.
- Une Task peut ne retourner aucune valeur (autre que son état).
- Une Task<montype> retourne des données de type “montype”.
