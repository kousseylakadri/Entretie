[Tout](https://cdiese.fr/angular-component/)
# @Component
![Alt text](1.png)

Le décorateur `@Component{()}` définit les métadonnées* de votre composant.
  - Le `sélecteur:` nous permet de définir comment Angular identifie lorsque le composant est utilisé en HTML.

*Une métadonnée est une « donnée qui fournit de l'information sur une autre donnée »
# OnInit et @Input()    
![Alt text](2.png)

- `OnInit` est un hook de cycle de vie qui est appelé après qu'Angular a initialisé toutes les propriétés liées aux données d'une directive. Lors de la phase de détection de changement.
- Le décorateur `@Input()` permet d’implémenter des paramètres d’entrée dans le composant enfant qu’on pourra initialiser à partir du composant parent.
## Exemple
![Alt text](7.png)
![Alt text](8.png)
# Constructeur [ici](https://www.telerik.com/blogs/angular-basics-angular-constructor-overview)
![Alt text](3.png)

- Un `constructeur` Angular est une fonction utilisée pour initialiser une application Angular. Le constructeur est **exécuté lors de la première création de l'application**, et il est responsable de la configuration de l'environnement Angular. Le constructeur peut être utilisé pour **injecter des dépendances, définir les valeurs par défaut pour les propriétés et exécuter tout autre code d'initialisation nécessaire**.
- Le préfixe `readonly` est utilisé pour rendre une propriété en lecture seule. Les membres en lecture seule sont accessibles en dehors de la classe, mais leur valeur ne peut pas être modifiée.
![Alt text](4.png)

![Alt text](5.png)
![Alt text](6.png)
