# Abstracts

Le dossier abstracts/ regroupe les outils et helpers Sass utilisés à travers le projet. Toutes les variables globales, les fonctions, les mixins et les placeholders devraient se retrouver dans ce dossier.

La règle générale concernant ce dossier est qu’il ne devrait pas retourner une seule ligne de CSS s’il était compilé seul. Ce ne sont ici que des helpers Sass.

_variables.scss
_mixins.scss
_functions.scss
_placeholders.scss

## \_index.scss

Avec la dépréciation du mot-clé `@use`, nous utilisons désormais les mots-clés `@use` et `@forward`. Contrairement à `@use`, l'ajout de résumés avec `@use` en haut du fichier `main.scss` ne les rend pas globalement accessibles à tout ce qui suit.

Pour cette raison, nous devons importer ces résumés à l'aide du mot-clé `@use` chaque fois que nous en avons besoin dans les fichiers individuels, de la même manière que nous importerions des utilitaires dans le monde JavaScript d'ailleurs.

C'est là que nous avons besoin du mot-clé `@forward`.

Nous pouvons créer un fichier `_index.scss`. Dans ce fichier, nous pouvons collecter tous les partiels abstraits avec le mot-clé `@forward` et réexporter tous les modules abstraits lorsque nous en avons besoin sous forme d'entrée singulière.

Reference: [Sass Guidelines](https://sass-guidelin.es/) > [Architecture](https://sass-guidelin.es/#architecture) > [Abstracts folder](https://sass-guidelin.es/#abstracts-folder)
