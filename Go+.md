# Projet Go+
## Input output
[Video Aide](https://www.youtube.com/watch?v=dbeYVr41NL4)
### @Input
`@Input` le décorateur marque la propriété comme propriété d'entrée. C'est-à-dire qu'il peut recevoir des données du composant parent.
### @Output
`@Output` décore la propriété en tant que propriété de sortie.Le composant enfant déclenche l'événement et transmet les données comme argument à l'événement. Le composant parent écoute les événements à l'aide de la liaison d'événements et lit les données.

## Validateur et validateur custom
## Reactiveform (directive , formArray , fromGroup, formBuilder)
[Aide lien](https://www.tektutorialshub.com/angular/angular-reactive-forms/)

[Aide video](https://www.youtube.com/watch?v=gXYCBICC7N4)

Les formulaires réactifs fournissent une approche basée sur un modèle pour gérer les entrées de formulaire dont les valeurs changent au fil du temps. 
#### Comment utiliser les formulaires réactifs
- Importer `import { ReactiveFormsModule } from '@angular/forms';`
- Créer un modèle de formulaire dans une classe de composants à l'aide de FormGroup, FormControl et FormArrays
- Créez le formulaire HTML ressemblant au modèle de formulaire.
- Lier le formulaire HTML au modèle de formulaire
## Quand faire une division des composantes (réutilisation, séparation des concepts )
## Service , injection de dépendance
[Aide lien](https://learn.microsoft.com/en-us/dotnet/core/extensions/dependency-injection)

[Aide lien](https://angular.io/guide/lifecycle-hooks)
## cycle de vie angular (à quoi sert ngonInit, ngOnchanges, ngAfterviewInit , ngOnDestroy, etc )
### ngonInit

```
export class LifecycleComponent implements OnInit {
  products: Product[] = [];
 
  constructor(private fakeService: FakeService) { }
 
  ngOnInit() {
    this.fakeService.getProducts().subscribe(products => {
      this.products = products;
    });
  }
}
```

### ngOnChanges
```
// implémentation de l'interface OnChanges
ngOnChanges(changes: SimpleChanges) : void {
    // logique du composant
}
 
// exemple de valeur
{
   "prop1":{
      "currentValue":2,
      "firstChange":false,
      "previousValue":1
   }
}
 
// interface du SimpleChanges
export interface SimpleChanges {
    [propName: string]: SimpleChanges;
}
```

### ngAfterviewInit 

```
@Component({
    selector: 'popup',
    template: '<div class="popup"><ng-content></ng-content></div>'
})
export class PopupComponent {
}
```

```
<popup><div>Afficher ce <span class="une-classe">contenu</span> dans le composant popup !</div></popup>
```

### ngOnDestroy

```

```

## Comment fonctionne les ngModule (imports, déclarations , providers)
## Lazyloading des components
## Stratégie d'url standard
## Libraire Rxjs (subject, observer , observable.
## Pourquoi éviter les nesteds subscribe, takeUtile , unsubscribe )
