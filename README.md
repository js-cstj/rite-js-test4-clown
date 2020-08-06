# Le "Rite de passage"
**But du rite de passage** : Démontrer que l'on est capable de suivre des instructions simples et d'extrapoler ces connaissances dans divers contextes. Pour surmonter le rite de passage, l'élève devra être capable de recomposer n'importe quelle arborescence de balises HTML donnée par le professeur.

## Étape 1 - La balise
Ajouter des balises simples une à la suite de l'autre.

### Les nouveaux mots-clés
**En résumé** : `getElementById`, `createElement`, `appendChild` et `innerHTML`
```javascript
//Récupérer l'élément HTML dont l'attribut id a la même valeur que un_id.
element = document.getElementById(un_id); 

// Créer un élément HTML (balise) vide dont le nom correspond à la valeur de une_balise
element = document.createElement(une_balise); 

// Ajouter un elementEnfant à la fin du contenu d'un elementParent
elementParent.appendChild(elementEnfant); 

// Définit le contenu HTML d'une balise
element.innerHTML = "<b>Un certain code HTML</b>"
```

## Étape 2 - Les attributs
Ajouter un attribut à des éléments nouvellement créés.

### Les nouveaux mots-clés
**En résumé** : `setAttribut`
```javascript
// Ajouter l'attribut unAttribut avec la valeur uneValeur à l'element
element.setAttribute(unAttribut, uneValeur);
```

## Étape 3 - Classes et styles
Les classes et les styles sont des attributs spéciaux : ils ont leurs propres mots-clés

### Les nouveaux mots-clés
**En résumé** : `classList.add` et `style._propriete_`
```javascript
// Ajouter la classe uneClasse à element
element.classList.add(uneClass);

// Ajouter une propriété CSS à element.
element.style._propriete_ = "valeur de la propriété"
```
**Note** : On remplacera la portion `_propriete_` par une version _camel case_ du nom de la propriété. Par exemple, on mettra `element.style.fontSize = "12px";` (à la place de `font-size`)

## Étape 4 - Imbrication
On doit maintenant imbriquer des balises nouvellement créées dans des balises créées précédemment.

### Les nouveaux mots-clés
Aucun

Il suffit de bien choisir l'élément auquel on applique le `appendChild`.