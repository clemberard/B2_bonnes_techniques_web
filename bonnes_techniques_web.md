# Bonnes techniques du web

## Sommaire

- Utilisation de Git


## Utilisation du versionning

### Qu'est ce que le versionning ?

Le versionning est un système qui permet de gérer les différentes versions d'un projet. Il permet de revenir à une version antérieure du projet, de voir les modifications apportées, de travailler à plusieurs sur un même projet, etc...

#### Importances du versionning

- Tracabilité des modifications : on peut voir qui a fait quoi et quand.
- Collaboration : plusieurs personnes peuvent travailler sur un même projet. Chacun peut travailler sur une fonctionnalité sans impacter le travail des autres.
- Sauvegarde : on peut revenir à une version antérieure du projet en cas de problème.
- Branching et merging : on peut créer des branches pour travailler sur une fonctionnalité sans impacter le travail des autres. On peut ensuite fusionner les branches entre elles.

Exemples de nomenclature de versionning :

Une des plus utilisées est la nomenclature SemVer (Semantic Versioning) : `MAJOR.MINOR.PATCH` :

- `MAJOR` : changement majeur, incompatible avec les versions précédentes.
- `MINOR` : ajout de fonctionnalités, compatible avec les versions précédentes.
- `PATCH` : correction de bugs, compatible avec les versions précédentes.

Exemple : `1.0.0` est la première version d'un projet. `1.0.1` est une version qui corrige un bug. `1.1.0` est une version qui ajoute une fonctionnalité. `2.0.0` est une version qui change complètement le projet.

### Utilisation de Git

Git est un logiciel de versionning. Il permet de gérer les différentes versions d'un projet. Il permet de revenir à une version antérieure du projet, de voir les modifications apportées, de travailler à plusieurs sur un même projet, etc... 

Il existe aussi d'autres logiciels de versionning comme SVN, Mercurial, etc...

#### Opérations et fonctionnalités

- checkout/update/commit : récupérer les modifications, envoyer les modifications, valider les modifications.
- branch/merge : créer une branche, fusionner les branches.
- atomic commit : soit toutes les modifications sont envoyées, soit aucune (garantie d'intégrité).

#### Performances

- Git est très performant avec des opérations locales rapides sur les versions et branches.

#### Réseau et collaboration

Git permet de travailler à plusieurs sur un même projet. Il permet de récupérer les modifications des autres et d'envoyer ses propres modifications. Il permet de gérer les conflits. Les fichiers sont stockés sur un serveur distant (GitHub, GitLab, BitBucket, etc...). Il est possible de travailler en local sans serveur distant.

#### Git config

La config de Git se fait avec la commande `git config`. Il est possible de configurer Git au niveau local ou global. La config locale est propre au projet. La config globale est propre à l'utilisateur.

- `git config --global user.name "John Doe"` : définir le nom de l'utilisateur.
- `git config --global user.email

#### Git init

La commande `git init` permet d'initialiser un projet Git. Elle crée un dossier `.git` qui contient les informations de versionning.

#### Git status

La commande `git status` permet de voir l'état du projet. Elle permet de voir les fichiers modifiés, les fichiers ajoutés, les fichiers supprimés, etc...

#### Git add

La commande `git add` permet d'ajouter des fichiers au prochain commit. Elle permet de préparer les fichiers à envoyer.

- `git add .` : ajouter tous les fichiers.
- `git add <fichier>` : ajouter un fichier.
- `git add -p <fichier>` : ajouter un fichier en mode interactif.

#### Git commit

La commande `git commit` permet d'envoyer les modifications. Elle permet de valider les modifications.

- `git commit -m "Message de commit"` : envoyer les modifications avec un message de commit.
- `git commit -a -m "Message de commit"` : envoyer les modifications de tous les fichiers modifiés avec un message de commit.

#### Git log

La commande `git log` permet de voir l'historique des commits. Elle permet de voir les informations des commits (hash, auteur, date, message, etc...).

#### Git diff

La commande `git diff` permet de voir les modifications apportées aux fichiers. Elle permet de voir les lignes ajoutées, modifiées ou supprimées.