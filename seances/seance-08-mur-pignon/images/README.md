# Images de la séance : seance-08-mur-pignon

Ce dossier doit contenir les schémas référencés dans le fichier `seance-08.tex`.

## Images attendues

- **`mur-pignon-vue-elevation.png`** — Vue en élévation du mur pignon : longueurs et niveaux
- **`mur-pignon-vent.png`** — Schéma d'application de l'action du vent sur le mur pignon
- **`mur-pignon-diagramme-rectangulaire.png`** — Schéma du diagramme rectangulaire de contraintes utilisé pour le calcul de $A_{cc}$
- **`mur-pignon-console-geometrie.png`** — Géométrie de la console courte au R+1 avec efforts du vent
- **`mur-pignon-console-bielles.png`** — Schéma de bielles et tirants de la console courte
- **`mur-pignon-console-ferraillage.png`** — Ferraillage de la console courte au R+1 (tirant, aciers répartis, anti-éclatement)

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

