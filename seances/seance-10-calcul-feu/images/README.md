# Images de la séance : seance-10-calcul-feu

Ce dossier doit contenir les schémas référencés dans le fichier `seance-10.tex`.

## Images attendues

- **`poutre-feu-coupes-ferraillage.png`** — Coupes de ferraillage de la poutre 30$\times$70 : section en travée (gauche) et sur appui B2 (droite)
- **`dalle-feu-ferraillage.png`** — Plan de ferraillage de la dalle nervurée — sections d'acier dans les deux sens

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

