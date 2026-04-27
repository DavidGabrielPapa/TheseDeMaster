# Projet de master

> Exploration du lien entre le profil psychologique MBTI et les relations entre acteurs.

---

## Description du projet

Tenter de répondre à cette question : **Existe-t-il un lien entre le type de personnalité MBTI d'un acteur et leurs relations entre eux ?**

L'analyse se déroule en trois étapes, chacune correspondant à un notebook dédié : exploration individuelle des deux bases de données, puis mise en commun et analyse croisée.

---

## Structure du projet

```
📦 TheseDeMaster/
│
├── datatest.ipynb       # Analyse de la base de données des acteurs
├── mbti.ipynb           # Analyse de la base de données MBTI des célébrités
├── graph.ipynb          # Croisement des deux bases & analyse des liens
│
├── Images/              # Graphiques exportés depuis les notebooks
│   └── Actors/
│        └── *.png
│   └── MBTI/
│        └── *.png
│   └── Graph/
│        └── *.png
│
└── README.md
```

---

## Notebooks

### `datatest.ipynb` — Analyse de la base de données des acteurs
Exploration et nettoyage de la base de données [Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) sur les acteurs. Ce notebook couvre :
- Aperçu général du dataset (dimensions, types, valeurs manquantes)

### `mbti.ipynb` — Analyse de la base de données MBTI
Exploration de la base de données [Kaggle](https://www.kaggle.com/datasets/yuraslastya/celeb-mbti) recensant les célébrités et leur type de personnalité MBTI. Ce notebook couvre :
- Aperçu général du dataset

### `graph.ipynb` — Croisement & analyse des liens
Fusion des deux bases de données et recherche d'un lien entre profil MBTI et relations d'acteur. Ce notebook couvre :
- Jointure et nettoyage des données croisées

---

## Sources de données

| Dataset | Source | Description |
|--------|--------|-------------|
| Acteurs | [Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) | Base de données sur les acteurs |
| MBTI Célébrités | [Kaggle](https://www.kaggle.com/datasets/yuraslastya/celeb-mbti) | Célébrités et leur type de personnalité MBTI |

---

## Lancer le projet

### Prérequis
- Python 3.13
- Jupyter Notebook


### Ordre d'exécution
1. `datatest.ipynb`
2. `mbti.ipynb`
3. `graph.ipynb`

---

## Dossier Images

Le dossier `Images/` contient tous les graphiques générés par les notebooks. Ils sont exportés automatiquement lors de l'exécution des cellules de visualisation.

---

## Librairies utilisées

| Librairie | Usage |
|-----------|-------|
| `kagglehub` | Téléchargement des datasets depuis Kaggle |
| `pandas` | Manipulation et analyse des données |
| `numpy` | Calculs numériques |
| `matplotlib` / `matplotlib.gridspec` | Visualisations et mise en page avancée des graphiques |
| `seaborn` | Visualisations statistiques |
| `networkx` | Construction et analyse de graphes |
| `scipy.stats` | Tests statistiques (chi2) |
| `collections` | Structures de données utilitaires (`Counter`, `defaultdict`) |
| `difflib` | Correspondance approximative de chaînes (`get_close_matches`) |
| `unicodedata` / `re` | Nettoyage et normalisation de texte |
| `json` | Lecture/écriture de fichiers JSON |
| `os` | Gestion des chemins et fichiers système |
