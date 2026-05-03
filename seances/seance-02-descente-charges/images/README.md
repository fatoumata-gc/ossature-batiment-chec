# Images de la séance : seance-02-descente-charges

Ce dossier doit contenir les schémas référencés dans le fichier `seance-02.tex`.

## Images attendues

- **`poteau-B2-position.png`** — Position du poteau B2 dans la vue en plan du bâtiment
- **`vue-elevation.png`** — Vue en élévation du bâtiment avec niveaux annotés
- **`surface-tributaire-B2.png`** — Surface tributaire du poteau B2 --- demi-portées des travées adjacentes
- **`coupe-planchers.png`** — Coupes-types des différents planchers

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

