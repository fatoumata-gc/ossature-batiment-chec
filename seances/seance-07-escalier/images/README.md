# Images de la séance : seance-07-escalier

Ce dossier doit contenir les schémas référencés dans le fichier `seance-07.tex`.

## Images attendues

- **`escalier-vue-plan.png`** — Vue en plan de l'escalier --- volées et palier intermédiaire
- **`escalier-coupe.png`** — Coupe en élévation de l'escalier --- paillasse, contremarche, giron
- **`escalier-schema-statique.png`** — Schéma statique de l'escalier --- charges projetées sur la longueur $L = 3{,}10$~m
- **`escalier-ferraillage-paillasse.png`** — Schéma de ferraillage de la paillasse --- armatures principales et armatures de répartition
- **`escalier-bequet-ferraillage.png`** — Schéma de ferraillage du béquet --- armatures principales et armatures de répartition

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

