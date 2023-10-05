# **Refont web : développement** 🚀 
![cover](./asset/cover.PNG)

>Ma mission aujourd'hui est de corriger toutes les erreurs et les problèmes présents sur cette page.

👉 [Résultat final](https://theocou.github.io/refontexo/)
## HTML
 Le premier problème est au niveau de la structure du code dans le index.html. En effet, la balise `main` n'est pas présente, elle est remplacée par une simple `div` avec une class `main` qui est très mal utilisée.Les balises `div` sont surutilisées des balises plus adaptées en terme de sémantique sont nécessaires. Un fichier PNG est présent en dehors du dossier `asset`.

Intéressons-nous maintenant plus en détail au code : suppression des liens dans les boutons. la partie `head` est beaucoup trop vide. Il manque des éléments tels que les balises `meta` :

```html
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="refont">
```

Un soucis d'accesibilité est aussi a résoudre, l'image en background ne s'adapte pas avec le format de l'écrans. Des problèmes de contrastes sont présents à plusieurs endroits de la page : en haut à droite dans la partie recherche (le texte n'est pas parfaitement visible a cause des couleurs), la couleur choisie pour le mot "Development" n'est pas bonne (contraste avec le fond), même chose pour le "Login Here".<br> Les `label` sont manquants sur les champs du form.

## CSS

Une erreur se trouve aussi dans le fichier de style css : un doublon `border-bottom-right-radius` dans le `.btn` est a supprmier. Il faut aussi convertir toutes les valeurs qui sont en `px` en `rem`.

## Charte graphique

Un travail de recherche a été fait afin de résoudre les problèmes de contraste.

### Après changements :

![preview](./asset/preview.PNG)