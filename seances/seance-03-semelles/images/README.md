# Images de la séance : seance-03-semelles

Ce dossier doit contenir les schémas référencés dans le fichier `seance-03.tex`.

## Images attendues

- **`semelle-deux-pieux-principe.png`** — Principe d'une semelle sur deux pieux --- vue en plan et coupe en élévation
- **`semelle-pieux-cote-bielle.png`** — Demi-coupe transversale --- méthode des bielles : effort N, bielle inclinée à $\theta = 55^{\circ}$, hauteur utile $d$
- **`semelle-pieux-ferraillage.png`** — Coupe en élévation du plan de ferraillage de la semelle sur deux pieux : armatures inférieures, supérieures, verticales et horizontales
- **`semelle-superficielle-coffrage.png`** — Coffrage de la semelle superficielle isolée 2,70 $\times$ 2,70 $\times$ 0,65~m
- **`semelle-superficielle-ferraillage.png`** — Plan de ferraillage de la semelle superficielle --- vue en plan et vue en élévation

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

