# 02 - Gimp pour réaliser des visuels avec de vraies illustrations.

Maintenant qu'on a appris à réaliser des visuels très simples (un slogan, un fond, un logo) dans le [précédent tutoriel](gimp_O1_Visuel_simple.md), on peut passer à l'étape suivante : des visuels avec de vraies images.

## Principe d'esthétique : le nombre d'or

L'œil humain est ainsi fait qu'il est particulièrement sensible à certaines proportions, et singulièrement au nombre d'or ϕ :

![La formule du nombre d'or](gimp_02_aux/01_nombre_or.jpg)

Cette formule est un peu abstraite. En fait, elle permet de définir un rectangle d'or, c'est à dire un rectangle dont le rapport de la longueur sur la largeur vaut ϕ :

![Un rectangle d'or](gimp_02_aux/02_rectangle_or.png)

Toujours trop abstrait ? Maintenant, jetons un œil à quelques joyaux de l'architecture :

![Temple d'or](gimp_02_aux/03_temple_or.jpg)

De l'histoire de l'art :

![Vierge d'or](gimp_02_aux/04_raphael_or.png)

Ou même du design :

![Pomme d'or](gimp_02_aux/05_apple_or.png)

On va donc essayer de suivre les proportions d'or en composant nos visuels pour avoir le même succès que Raphaël ou Steve Jobs ^^ Notre but va donc être de disposer les différents éléments du visuel dans les rectangles d'or, en jouant sur leur taille pour que l'ensemble paraisse harmonieux.

Évidemment, Gimp fournit ce qu'il faut pour ça.

## Ouvrir une image.

Supposons que nous voulions faire un visuel pour saluer la solidarité médicale de Cuba. On veut mettre en exergue la citation "Nous larguerons des médecins, pas des bombes", qui décrit cette démarche et que Fidel Castro a prononcée dans les années 80.

On commence par chercher une belle photo qui se prête à ce genre de message. Disons celle-ci :

![Fidel](gimp_02_aux/05_castro.jpg)

On la charge dans Gimp (Fichier ⟶ Ouvrir) et on commence par la manipulation qu'on a déjà faite la dernière fois : Calques ⟶ Transparence ⟶ Ajouter un canal alpha.

## Redimensionner l'image.

Ensuite, dans le panneau des outils, on sélectionne l'outil de sélection rectangulaire, en précisant "sections d'or" dans le menu des guides (indiqué par la flèche rouge) :

![Sections d'or](gimp_02_aux/06_sections_or.png)

On encadre l'image avec la sélection régulière, ce qui fait apparaître les guides :

![Guides](gimp_02_aux/07_guides.png)

Visiblement, aucune section d'or ne permet d'écrire correctement notre texte : ce serait vraiment très petit, ou il faudrait écrire par-dessus l'image.
Qu'à cela ne tienne, nous allons la redimensionner. Élargissons notre sélection de manière à ce que la photo de Castro soit à la gauche d'un rectangle d'or (nous écrirons le texte à sa droite) :

![Guides redimension](gimp_02_aux/08_guides_redimension.png)

On remarque que notre nouvelle image devra mesurer 848 pixels de largeur.

![Valeurs redimension](gimp_02_aux/09_redimension_pixels.png)

On clique sur Image ⟶ Rogner selon la sélection (qui supprime la partie superflue de l'image), puis sur Image ⟶ Taille du canevas. Il n'y a plus qu'à sélectionner notre nouvelle largeur et à indiquer que tous les calques doivent être redimensionnés :

![Redimensionner](gimp_02_aux/10_taille_canevas.png)

## Boucher les trous.

Évidemment, la partie droite de l'image est maintenant transparente. On veut la colorier de la même couleur d'arrière-plan que la photo : un "presque noir".
Rien de plus simple, il suffit de sélectionner l'outil Pipette :

![Pipette](gimp_02_aux/11_pipette.png)

Et de cliquer sur une zone de l'image qui a la couleur désirée. Il ne reste plus qu'à colorier la partie transparente de l'image, en utilisant l'outil Pot de peinture, comme on l'a déjà vu :

![Coloriage](gimp_02_aux/12_coloriage.png)

## Ajouter le texte et le logo en suivant les sections d'or

En utilisant l'outil de sélection rectangulaire, on repère les sections d'or et on les utilise pour positionner le texte (ici, on utilise la police [Bebas Neue](https://www.dafont.com/fr/bebas-neue.font) pour la citation, et [Ubuntu](https://design.ubuntu.com/font/) pour le nom de Castro) :

![Résultat](gimp_02_aux/13_resultat.png)

Il n'y a plus qu'à enregistrer l'image et à l'exporter en png.
Une image comme celle-là marchera très bien, la preuve :

![Post](gimp_02_aux/14_post.png)
