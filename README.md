# Tuto_Angular

## Partie 1 : Initiation

#### 1.1 Create the product list
1.1.1
*ngFor  un peu comment  boucle for dans JS,  ici ajouter `<div>` pour chaque produit dans products (Dans ses `<div>` affiche name of produit (ici `{{ product.name }}`) en form h3) into DOM. 
```
<div *ngFor="let product of products">

  <h3>
      {{ product.name }}
  </h3>

</div>
```
un peu equivalant JS:
```
for (let produit of produits){
    content+=`
        <div>
            <h3>
                ${produit.name}
            </h3>
        </div>`
}
```

1.1.2
```
<a [title]="product.name + ' details'">
```
[] permettre binding propréte avec data,  ici propréte "title" de <a> binding avec String name of produit + String details

un peu equivalent:
```
<a title="${product.name} details">
```

1.1.3
*ngIf condition un peu comment  if dans JS. 
```<p *ngIf="product.description">
    Description: {{ product.description }}
  </p>
```
ici si product.product.description n'exist pas (condition est false)
<p></p>sera pas créer

1.1.4
```
 <button (click)="share()">
    Share
  </button>
```
ici event click lien avec method share(), si on click button "Share",  it will call method share()

#### Pass data to a child component




## Partie 2 : Routing

## Partie 3 : Data

## Partie 4 : Formulaire