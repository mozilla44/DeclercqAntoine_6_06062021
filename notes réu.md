# Notes - Réunion client FishEye

## Entreprise :

Site web de photographes freelances.
_“Nos clients prennent de super photos, mais ils n’y connaissent rien en développement web. C'est
pourquoi nous proposons une plateforme unique pour montrer leurs photos sur une belle page
et les contacter pour des événements ou des tirages. Nous sommes l'un des plus grands sites de
photographie en freelance, avec un énorme réseau de photographes.”_

## Objectif :

Leur site est obsolète et a besoin d'être remanié.
_"Notre site a été construit il y a plus de dix ans, et nous n'avons pas eu l'occasion de le mettre à
jour jusqu'à présent. Nous venons de lever des fonds et nous aimerions que votre équipe le
transforme d'un site statique à un site dynamique"._

## Prototype des fonctionnalités :

Nous devons créer les pages suivantes pour le prototype :
● Page d'accueil :
○ Liste de tous les photographes avec leur nom, leur slogan, leur localisation,
leur prix/heure, leurs tags et une image miniature de leur choix.

○ Lorsque l'utilisateur clique sur la vignette d'un photographe, il est amené à sa
page.
● Pages des photographes (une pour chaque photographe échantillon) :
○ Affiche une galerie des travaux du photographe.
○ Les photographes peuvent montrer à la fois des photos et des vidéos.
■ Dans le cas des vidéos, montrer une image miniature dans la galerie.
○ Chaque média comprend le titre, la date, le prix et le nombre de clichés.
■ Lorsque l'utilisateur clique sur l'icône "Like", ça incrémente le nombre
de likes affiché.
■ Le nombre total de clichés doit être compté et ajouté au total du profil
du photographe.

○ Les médias peuvent être triés par popularité, date ou titre.

○ Lorsque l'utilisateur clique sur un média, celui-ci doit s’ouvrir dans une
lightbox :
■ Lorsque la lightbox est affichée, il y a une croix dans le coin pour
fermer la fenêtre.
■ Des boutons de navigation permettent de passer d'un élément média
à l'autre (les utilisateurs peuvent cliquer sur ces boutons pour
naviguer).
■ Les touches fléchées permettent également de naviguer entre les
médias.
○ Afficher un bouton pour contacter le photographe.


```
■ Le formulaire de contact est une modale qui s'affiche par-dessus le
reste.
■ Il comprend des champs pour les noms, l'adresse électronique et le
message.
■ Plus tard, le bouton de contact enverra un message au photographe.
Pour l'instant, seulement afficher le contenu des trois champs dans
les logs de la console.
```
## Exigences design supplémentaires

**Rendre le système mobile convivial et responsive**
_"Veillez à ce que toutes les pages soient responsives et s'adaptent bien aux smartphones ainsi
qu'aux écrans de bureau. Peu de nos utilisateurs visitent le site sur des tablettes, donc vous
n'avez pas besoin de concevoir pour cette taille d'écran"._
**L'accessibilité est clé!**
_"Il est très important que notre site soit accessible aux utilisateurs malvoyants. ​Toutes nos
photos doivent comporter des descriptions textuelles​, et vous devez les inclure dans la page. De
plus, l'utilisateur doit pouvoir ​utiliser les commandes du clavier pour naviguer sur le site, comme
les touches fléchées de la lightbox​"._
● Utilisez des éléments HTML "sémantiques" qui décrivent leur intention autant que
possible, au lieu de mettre des éléments <div> et <span> partout.
● Lorsque vous devez créer un élément personnalisé, ajoutez des attributs ARIA pour
décrire ce qu'il fait.
● Le code devrait passer les tests ​AChecker​ sans “known issue” (afin qu'il soit
conforme aux WCAG).
● Toute la gestion des événements (par exemple, les clics et les pressions au clavier)
doit être configurée (utilisez KeyboardEvent.key ou KeyboardEvent.code.).
● Utilisez un ​lecteur d'écran gratuit​ pour vous faire une idée de ce que représente
l'utilisation du site pour une personne malvoyante.


