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