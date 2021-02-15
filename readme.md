# Introduction

L'objectif du document est la création d'une *cheat sheet* ou "feuille de triche". 

L'ensemble des fonctions que vous devez documenter se trouvent dans ce document, à vous de  remplir les espaces vides 😉

Ce document pourra vous suivre tout au long de vos études, n'hésitez à le compléter au fur et à mesure.

---

Pour compléter le document, vous utiliserez la fonction **fork** de GitHub pour copier ce projet dans votre espace personnel.

[Si besoin, rendez-vous dans ce dépôt pour revoir les bases de Javascript](https://github.com/Maxence-Machu/javascript-basic-memo)

---

## La fonction GetElementByID()

### Que fait la fonction ?
La méthode getElementById() renvoie un objet qui représente l'élément dont la propriété  id correspond à la chaîne de caractères spécifiée.
Étant donné que les ID d'élément doivent être uniques, s'ils sont spécifiés, ils constituent un moyen utile d'accéder rapidement à un élément spécifique.

### Pourquoi l'utiliser ?
La fonction getElementById doit être utilisée si l'on veut utiliser un élément du DOM en HTML grâce à Javascript 

#### Note supplémentaire
La fonction getElementByID est à ne pas confondre avec la fonction *getElementsByClassName*. 
Les ID dans une page web sont uniques, on ne peut donc pas récupérer plusieurs éléments avec cette fonction. 

### Exemple de code:
```javascript
let element = document.getElementByID('mon-element');
console.log(element);
```

## La fonction GetElementsByClassName()

### Que fait la fonction ?
Retourne la liste de tous les éléments HTML du DOM ayant la classe indiquée en paramètre

### Pourquoi l'utiliser ?
La fonction GetElementsByClassName() doit être utilisée si l'on veut utiliser un élément du DOM en HTML grâce à sa class

### Exemple de code:
```javascript
var x = document.getElementsByClassName("example");
});
```

## La fonction querySelector() et querySelectorAll()

### Que fait la fonction ?
Retourne le premier élement parmi les descendant de l'élement sur lequel on l'invoque qui correspond au groupe de sélecteurs spécifiés.

### Pourquoi l'utiliser ?
Si le sélecteur correspond à un ID et que cet ID est utilisé de façon erronée plusieurs fois dans le document, le premier élément en correspondance est retourné.

### Exemple de code:
```javascript
element = document.querySelector(sélecteurs);
```

## La fonction addEventListener()

### Que fait la fonction ?
La méthode addEventListener() d'EventTarget installe une fonction à appeler chaque fois que l'événement spécifié est envoyé à la cible.

### Pourquoi l'utiliser ?
Pour définir des actions à chaque fois q'un évenement se produit

### Exemple de code:
```javascript
function gestionnaireDEvenement(evenement) {
  if (evenement.type == fullscreenchange) {} 
  else /* fullscreenerror */ {}
}
```

## La fonction stopPropagation()

### Que fait la fonction ?
Évite que l'évènement courant ne se propage plus loin dans les phases de capture et de déploiement.

### Pourquoi l'utiliser ?
Stopper la propagation d’un évènement va pouvoir s’avérer très pratique dans le cas où nous avons plusieurs gestionnaires d’évènements pour le même évènement attachés à différents éléments dans la page et où on souhaite n’exécuter que le gestionnaire le plus proche de l’élément cible de l’évènement.

### Exemple de code:
```javascript
function func1(event) {
  alert("DIV 1");
  event.stopPropagation();
}
```

## La fonction addEventListener('mousemove', maFonction)

### Que fait la fonction ?
La méthode addEventListener() d'EventTarget installe une fonction à appeler chaque fois que l'événement spécifié est envoyé à la cible.

### Pourquoi l'utiliser ?
Ajouter une fonction à un élement précis

### Exemple de code:
```javascript
document.addEventListener("mousemove", maFonction);
```

## La fonction parseInt()

### Que fait la fonction ?
La fonction parseInt() analyse une chaîne de caractère fournie en argument et renvoie un entier exprimé dans une base donnée.

### Pourquoi l'utiliser ?
Permettre de convertir une chaîne en nombre entier. exemple (affichage 2+2 avec ParseInt ça affiche 4)

### Exemple de code:
```javascript
let saisie= "2";
document.write(parseInt(saisie)+2);
```


## La variable "event" dans le code suivant:

### Code:
```javascript
element.addEventListener('event-name', function(event) {
  console.log(event);
});
```

### Qu'est-ce que cette variable ?
la variable event est la fonction définie que va executer "event-name" lorsque que cet evenement se produira

### Pourquoi l'utiliser ?
Ajouter une fonction à un élement précis


