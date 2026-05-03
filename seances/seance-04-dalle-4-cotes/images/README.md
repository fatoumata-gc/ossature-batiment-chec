# Images de la séance : seance-04-dalle-4-cotes

Ce dossier doit contenir les schémas référencés dans le fichier `seance-04.tex`.

## Images attendues

- **`dalle-sur-4-cotes.png`** — Dalle sur 4 côtés au 1\textsuperscript{er} sous-sol --- vue en plan avec dimensions $l_x = 3{,}05$~m et $l_y = 5{,}85$~m
- **`dalle-diffusion-45.png`** — Diffusion à $45^{\circ}$ de la charge concentrée sur le feuillet moyen --- $u = u_0 + h$, $v = v_0 + h$
- **`dalle-repartition-moments.png`** — Répartition des moments en travée et sur appuis --- diagrammes en X et en Y
- **`dalle-plan-ferraillage.png`** — Plan de ferraillage de la dalle --- disposition des armatures dans les deux directions

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

