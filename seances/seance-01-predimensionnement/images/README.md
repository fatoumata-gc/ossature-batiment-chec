# Images de la séance : seance-01-predimensionnement

Ce dossier doit contenir les schémas référencés dans le fichier `seance-01.tex`.

## Images attendues

- **`predim-vue-plan-batiment.png`** — Vue en plan de la partie infrastructure du bâtiment : files A, B, C et 1 à 6 ; portées $L = 6{,}50$~m et $\ell = 6{,}00$~m
- **`predim-poutre-secondaire-charges.png`** — Distribution des charges sur la poutre secondaire (surfaces afférentes trapézoïdales)
- **`predim-poutre-principale-charges.png`** — Schémas de distribution des charges sur la poutre principale : modèle complet (gauche) et simplifié (droite)

## Procédure d'ajout

Une fois l'image préparée :

1. Placer le fichier `<nom>.png` dans ce dossier (`images/`).
2. Dans le fichier `.tex` parent, remplacer la ligne :
   ```latex
   \figureplaceholder{<nom>}{<légende>}
   ```
   par :
   ```latex
   \begin{figure}[H]\centering
     \includegraphics[width=0.7\linewidth]{<nom>.png}
     \caption{<légende>}\label{fig:<nom>}
   \end{figure}
   ```

