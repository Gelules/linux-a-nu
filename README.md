# Linux à Nu : Dissection d’un système moderne par le code

Bienvenue dans **Linux à Nu : Dissection d'un système moderne**, un livre
technique et pédagogique qui explore le système Linux depuis ses fondations
jusqu’à ses couches les plus avancées, uniquement à travers du **code**, de
l’**expérimentation**, et de la **manipulation directe**.

## Objectif

Ce projet vise à rendre compréhensible — et accessible — l’ensemble des
mécanismes d’un système GNU/Linux, en partant **du shell** jusqu’au **noyau**,
en passant par :

- la programmation système en C et assembleur ;
- les modules du noyau et la compilation du kernel ;
- le réseau, les conteneurs, l’administration système ;
- l’OSDev (développement d’un OS from scratch) ;
- le reverse engineering et l’instrumentation.

## Organisation du dépôt

```
.
├── source/             # Fichiers .rst du livre (Sphinx)
│   ├── index.rst       # Table des matières
│   ├── 01-prise-en-main.rst
│   └── ...
├── build/              # Fichiers générés par Sphinx
├── requirements.txt    # Dépendances Python (Sphinx + thème)
├── Makefile            # Commandes de build HTML/PDF
├── README.md           # Ce fichier
└── TODO                # La liste des choses à faire
```

## Construire le livre

### 1. Installer les dépendances

Assurez-vous d’avoir Python, `pip` et `make` installés, puis :

```bash
pip install -r requirements.txt
```

### 2. Générer la documentation

La documentation est, après génération, disponible dans le répertoire **build**.

#### HTML

Depuis la racine du dépôt (où se trouve le Makefile), exécutez :
```bash
make html
```

#### HTML en une seule page

Depuis la racine du dépôt (où se trouve le Makefile), exécutez :
```bash
make singlehtml
```

#### LaTeX

Depuis la racine du dépôt (où se trouve le Makefile), exécutez :
```bash
make latex
```

#### PDF par LaTeX

Depuis la racine du dépôt (où se trouve le Makefile), exécutez :
```bash
make latexpdf
```
#### Autre
Pour savoir les autres formats que Sphinx peut générer, depuis la racine du
dépôt (où se trouve le Makefile), exécutez :
```bash
make
```
