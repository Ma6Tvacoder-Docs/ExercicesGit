# Hello World

*Traduction française de la page* [Hello World](https://guides.github.com/activities/hello-world/ "version original")

*Ce tutoriel ne prend qu'une dixaine de minutes à completer*

*Auteur* [@adricen](https://github.com/adricen "version original")

Le projet Hello World est un classique du monde de la programmataion. C'est un exercice simple qui vous permet d'apprendre quelque chose de nouveau. Commençons avec GitHub!

## Qu'est-ce que GitHub ?

GitHub est un hebergeur de code, de control de versionning et de collaboration. Il vous permet ainsi qu'a d'autres de travailler ensemble sur des projets, de nimporte où.
Ce tutoriel vous apprend l'essentiel comme les *repository*, *branches*, *commits* et les *Pull Requests*. Vous allez creer votre propre Hello World repository et apprendre la methode de travail avec les *Pull Request*, une methode populaire pour creer et visionner du code.

### Pas de code necessaire

Pour completer ce tutoriel vous aurez besoin d'un [compte GitHub.com](https://github.com/) et d'une connexion internet. Vous n'avez pas besoin de savoir coder, utiliser les lignes de commande ou installer Git ( le logiciel de control de version GitHub est en place ).

> **Astuce :** Ouvrez ce guide dans une fenêtre à part ( ou un onglet ) afin que vous puissiez voir toutes les étapes points par points de ce tutorial.

## Etape 1. Creer un *Repository*

Un **Repository** ou repertoire, est en général utilisé pour organiser un projet simple. Le **repository** peut contenir des dossiers et des fichiers, des vidéos, des notes et des ensembles de données -- tout ce dont votre projet à besoin. Il est recommendé de mettre un fichier Readme, ou un fichier avec les informations relative à votre projet. GitHub vous rend la tache facile en vous proposant d'en ajouter un au même moment que lorsque vous creer votre **repository**. *Il vous offre également la possibilité de creer un fichier de license*.

Votre repertoire `hello-world` peut être un endroit ou vous stoquez des idées, des ressources, ou même partagez et discutez des choses avec les autres.

### Creer un nouveau repertoir / *repository*

1. Dans le coin supperieur droit, à côté de votre avatar ou *identicon*, cliquez + et selectionne *New repository*
2. Nommez votre repertoir **hello-world**
3. Ecrivez une courte desciption
4. Selecionnez *Initialize this repository with a README*
![Explication 01](https://guides.github.com/activities/hello-world/create-new-repo.png "Explenation01")
5. Cliquez sur *Create repository*

## Etape 2. Creez une Branch

Creer une branche ou *branching* est un moyen de travailler sur differentes versions d'un repertoire en même temps.

Par defaut votre repertoire a une branche nommé **master**, concidéré comme la branche principale. Nous utiliserons les branches pour experimenter et editer le projet avant de les envoyer sur le **master**.

Quand vous créez une branche à partir du repertoir **master**, vous faitent une copie, ou une *photo* de master comme si c'était le point de départ à ce moment là. Si quelqu'un d'autre fait un changement sur la branche **master** pendant que vous travaillez sur votre branche, vous pouvez retirer les elements avec la commande *pull* de ces updates.

Ce diagramme montre :

+ La branche **master**
+ une nouvelle branche appelé **feature** ( car nous allons travailler sur une nouvelle fonctionnalité dans cette branche )
+ Le parcour que **feature** prend avant de *merge* ( fusionner ) la branche dans **master**
![Explication 02](https://guides.github.com/activities/hello-world/branching.png "Explenation02")
Avez vous déjà sauvegardé une version differente d'un fichier ? Quelque chose comme :
+ **histoire.txt**
+ **histoire-joe.txt**
+ **histoire-joe-edit-reviewed.txt**
Les branches accomplissent un travail similaire dans le repertoir GitHub

Ici à GitHub, nos developpeurs, ecrivains et designers utilisent les branches pour sauvegarder les *patchs* ( ou *bug fix* ) et les *feature work* (complements) séparé de la branche **master** ( que l'on apel production ). Quand un changement est prêt, ils mergent leur branche dans **master**.

### Pour creer une nouvelle branche

1. Aller dans votre nouveau *repository* / repertoire
2. Cliquez sur la liste déroulante en haut de la liste de fichier ou est ecrits **branch: master**
3. Tapez le nom de votre branch, **readme-edits** dans la boite de dialogue *new branch*
4. Selectionnez la boite de dialogue bleu *Create branch* ou appuyez sur **entrer**
![Explication 03](https://guides.github.com/activities/hello-world/readme-edits.gif "Explenation03")

Maintenant vous avez 2 branches, une **master** et une autre **readme-edits**. Elles sont exactement pareil pour le moment, mais plus pour longtemps. Ensuite nous nous allons ajouter des changements a notre nouvelle branche.

## Etape 3. *Make and commit changes*

Bravo!
Maintenant vous êtes dans la vue de votre branche **redme-edits** qui est une copie de la branche **master**. Faisons quelques modifications.

Sur GitHub, sauvegardez vos changements, et appuyez sur commits. A chaques commit et associé un message de commit qui est une description ou explication de pourquoi à été fait un changement en particulier. Le message de commit permet de retrouver son commit dans un historique de commit, il vous permet de revenir en arriere si besoin et de ne pas être perdu. Il vous permet donc de comprendre ce qu'est ce message de commit.

### *Make and commit changes*

1. Cliquez sur le fichier **README.md**
2. Cliquez sur l'icon crayon dans le coin supperieur droit du lecteur de fichier pour l'editer
3. Dans l'editeur, ecrivez un morceau à propos de vous
4. Ecrivez un message de commit qui decris vos changements
5. Cliquez sur le bouton `commit changes`
![Explication 04](https://guides.github.com/activities/hello-world/commit.png "Explenation04")

Ces changements seront fait uniquement sur le fichier README sur votre branche **readme-edits**, donc maintenant le contenus de cette branche est different de la branche **master**.

## Etape 4. Faire un Pull Request

*Superbe modification!*
Maintenant que vous avez fait ce changement de la branche **master** vous pouvez faire un *Pull Request*.

Le *Pull Request* est au coeur de la collaboration sur GitHub. Quand vous demandez un *Pull Request*, vous proposez vos changements et demandez que quelqu'un valide, prennent votre contribution et la fusionne dans sa branche. *Pull Request* montre les differences de contenus entre les deux branches. Les changements, ajouts, suppretions sont montrés en vert ou rouge.

Dés que vous avez fait un *commit*, vous pouvez demander un *Pull Request* et commencer une discution avant même que le code soit finis.

En utilisant le [systeme de @mention](https://help.github.com/articles/about-writing-and-formatting-on-github/#text-formatting-toolbar "mentionner quelqu1") de GitHub dans votre message de *Pull Request*, vous pouvez demander un retour d'une personne en particulier ou même à une équipe, qu'elle soit en bas de léimmeuble comme au bout du monde.

Vous pouvez même demander un *Pull Request* dans votre propre repertoire / *repository* et fusionner / *merge* les fichiers vous même.

### Demander un *Pull Request* pour changer le fichier README

*Cliquez sur l'image pour une version plus large*

Colons can be used to align columns.

| Points        | Rendus           |
| ------------- | ---------------- |
| Cliquez sur le bouton *Pull Request*, ensuite depuis la page  *Pull Request*  cliquez sur le bouton vert  *New Pull Request*  | ![Explication 05](https://guides.github.com/activities/hello-world/pr-tab.gif "Explenation05") |
| col 2 is      | centered      |
| zebra stripes | are neat      |
