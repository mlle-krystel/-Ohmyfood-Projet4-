# Pages

Si vous avez des styles spécifiques à certaines pages, il est préférable de les inclure à l’intérieur d’un dossier pages/ dans un fichier portant le nom de la page. Par exemple, il n’est pas rare d’avoir des styles très spécifiques pour la page d’accueil, d’où la nécessité d’un fichier _home.scss dans pages/.

_home.scss
_contact.scss

*Note — Depending on your deployment process, these files could be called on their own to avoid merging them with the others in the resulting stylesheet. It is really up to you.*

Reference: [Sass Guidelines](https://sass-guidelin.es/) > [Architecture](https://sass-guidelin.es/#architecture) > [Pages folder](https://sass-guidelin.es/#pages-folder)
