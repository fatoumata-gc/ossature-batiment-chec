# Rapport — Ossatures de bâtiments

[![Build LaTeX & Deploy](https://github.com/fatoumata-gc/ossature-batiment-chec/actions/workflows/build.yml/badge.svg)](https://github.com/USER/ossature-batiment-chec/actions/workflows/build.yml)

Rapport du projet **Ossatures de bâtiments** - CHEBAP/TS - Fatoumata Bineta SALL - Année universitaire 2025-2026 - Chargé de TD : M. Bodet.

> 📄 **Le PDF compilé est disponible en ligne :** [Lien GitHub Pages](https://fatoumata-gc.github.io/ossature-batiment-chec/) 

---

## Structure du dépôt

```
ossature-batiment-chec/
├── main.tex                          # Document principal (orchestrateur)
├── preambule.tex                     # Préambule LaTeX (packages, commandes)
├── meta/
│   ├── page-de-garde.tex             # Page de titre
│   ├── enonce.tex                    # Énoncé du projet (à compléter)
│   ├── enonce.pdf                    # Scan de l'énoncé (à ajouter)
│   └── synthese-resultats.tex        # Tableaux de synthèse finaux
├── seances/
│   ├── seance-01-predimensionnement/
│   │   ├── seance-01.tex
│   │   └── images/                   # Schémas de la séance
│   ├── seance-02-descente-charges/
│   ├── seance-03-semelles/
│   ├── seance-04-dalle-4-cotes/
│   ├── seances-05-06-poutre/
│   ├── seance-07-escalier/
│   ├── seance-08-mur-pignon/
│   ├── seance-09-mur-sous-sol/
│   ├── seance-10-calcul-feu/
│   └── seances-11-12-plancher-dalle/
├── .github/workflows/
│   └── build.yml                     # CI : compilation + déploiement
└── README.md
```

## Compilation locale

Si une distribution LaTeX (TeX Live ou MiKTeX) est installée :

```bash
pdflatex main.tex
pdflatex main.tex      # deuxième passe pour la table des matières
```

Ou avec `latexmk` :

```bash
latexmk -pdf main.tex
```

Le PDF généré s'appelle `main.pdf`.

## Compilation automatique (CI/CD)

Le dépôt utilise **GitHub Actions** pour compiler le rapport automatiquement à chaque modification :

1. **À chaque push sur `main`** : le PDF est compilé et publié sur **GitHub Pages**, accessible à l'URL ci-dessus.
2. **À chaque push sur une branche** : le PDF est compilé et disponible en **artifact** de build (téléchargeable depuis l'onglet Actions, conservé 90 jours).
3. **Sur création d'un tag de version** (par exemple `v1.0`) : une **release GitHub** est créée automatiquement avec le PDF en pièce jointe.

### Créer une release versionnée

```bash
git tag -a v1.0 -m "Première version finale du rapport"
git push origin v1.0
```



