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

![Alt text](3.png)
![Alt text](4.png)

![Alt text](5.png)
![Alt text](6.png)
