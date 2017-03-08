# Lignes de Commandes de GitBash

Afin de commencer à travailler correctement sur Git il vous sera nécessaire de connaître quelques commmandes de base qui vous permettrons d'aller plus loin.
les valeurs placé <> seront des choses à remplacer par votre code.

## Configurer son GitBash

### Configuration

Il est important de lier votre compte a GitHub pour que vos actions asoient contabilisé et mise a jour sur votre profil. S'aisissez vous de votre userName github et de l'adresse mail lié a votre compte GitHub

Afin de les configurer dans GtiBash vous devrez faire ces deux commandes :

    git config --global user.name "John Doe"
    git config --global user.email "johndoe@example.com"

### L'aide

Sur chaque commandes, il est possible d'afficher l'aide en ligne directemenet depuis la console avec la commande

    --help

En tapant par exemple

    git commit --help

Une page sur la commande devrait s'ouvrir vous donnant les inforamtions principales relatives a cette commande.

### Navigation

Pour naviguer dans les dossier vous utiliserz les commandes suivantes :

    ls --> lister les contenus du dossier courant
    cd < nom du dossier > --> renter dans le dossier de votre choix
    cd .. --> revenir en arriere dans la hierarchie

Avec ces 3 commandes vous devez pouvoir naviguer en toute liberté sur votre ordinateur en ligne de commandes

## Les commandes Git

### Cloner

Lorsque vous voudrez commencer à travailler sur un projet git il vou sera necessaire de le 'cloner' afin d'avoir les dossier en locale et de pouvoir travailler dessus.
Je vous conseil de créer un dossier Git dans votre dossier htdocs dans lequel vous 'clonerez' tous vos dossiers proprement à cet endroit.
Vous utiliserez la commande 'git clone'

    git clone < le lien vers votre projet >

Cela telechargera les dossier sur votre ordinateur en créant un dossier caché .git dans lequel se trouve le liens vers la base online et toutes les données concernant votre participation a ce projet.

### Status

Pour savoir ou vous en êtes dans le code, utilisez la commande

    git status

Cela vous renvera un message vous donnant la direction a suivre. Soit votre projet est a jour, soit vous avez des choses a commiter online ou peut-être des conflis... ainsi de suite.
Cette commande est une des principales que vous utiliserez.

### Pull

Lorsque l'on veut actualiser son dossier en locale on utilise la commmandes

    git pull origin master

    git --> on signifie a Git que l'on fait appel à lui
    pull --> on va utiliser la commande pull ou 'recuperer'
    origin --> on signifie a Git que l'on va travailler sur le dossier initial pas sur une branche
    master --> on est sur la branche principale, le master

Faire un git pull vous sera demandé a chaque fois que votre dossier en locale ne sera pas le meme que celui online. Si d'autres personnes travaillent avec vous il vous sera demandé de faire un pull avant de pouvoir pusher quoi que ce soit.
Il est possible que vous ayez des problem de merge si des changements trop important ont été fait. Se reporter a la section merge dans ce cas là.

### Add

Avant de faire un commit ou aprés avoir fait un pull, il faut ajouter au commit les fichiers nouvellement créé, soit ceux qui ne sont pas encore pris en compte dans le `commit`.

```git

git add .

```

### Commit

Losrque l'on à avancé sur son travail en locale et que l'on souhaite mettre à jour les document en ligne on utilise les commandes suivante

    git commit -am'message de commit'

    git --> signifier à Git que l'on fait appel à lui
    commit --> la commande que l'on demande à Git d'executer
    *-* --> option de la commande courante
    a --> a pour *all* On signifie au commit que l'on ne fait pas d'exeptions de fichiers
    m'message de commit' --> on ajoute un message au commit.

Si vous oubliez la commande -m une nouvelle fenêtre Vim ( editeur de texte de bash ) devrait s'ouvrir en vous proposant d'ecrire un message. Rentrez votre message et appuyer sur *:x* pour quitter et enregistrer.

### Push

Une fois que vous avez fait votre commit il est necessaire de faire un push afin d'update vos fichier online.
Pour ce faire on va utiliser cette commande :

    git push origin master

### Branch

Lorsque vous voulez travailler sur une partie precisement et rajouter du code sans prendre le risque de rendre tout votre code ineficace en cas d'erreur, il vous sera necessaire de creer une branche.

Deux methodes existent pour cela. Vous pouvez ecrire

    git branch <nom de votre branche>
    git checkout -b <nom de votre branche>

Une nouvelle branche va être créé Il vous faudra maintenant basculer dessus si vous n'êtes pas passé par la commande 'checkout'

### Checkout

pour changer de branches on va utiliser la commande

    git checkout <nom de la branche>

Il faudra remplacer 'origin master' par 'origin <nom de votre branche>' lorsque vous ferez un commit ou un pull en particulier ou quoi que ce soit d'autre.
