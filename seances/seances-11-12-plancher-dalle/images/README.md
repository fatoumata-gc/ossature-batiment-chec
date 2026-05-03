# Images de la séance : seances-11-12-plancher-dalle

Ce dossier doit contenir les schémas référencés dans le fichier `seances-11-12.tex`.

## Images attendues

- **`plancher-dalle-vue-3d.png`** — Vue d'ensemble du plancher-dalle étudié
- **`plancher-dalle-vue-en-plan.png`** — Vue en plan du plancher-dalle, file 2 dans le sens $y$, portées et console
- **`plancher-dalle-repartition-bandes.png`** — Répartition des moments en bandes (sur poteaux et centrales)
- **`plancher-dalle-armatures-final.png`** — Schéma de répartition des sections d'aciers retenues, par bande
- **`poinconnement-contour-controle.png`** — Contour de contrôle $u_1$ et zone d'armatures de poinçonnement

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

