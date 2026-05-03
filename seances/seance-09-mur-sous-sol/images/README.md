# Images de la séance : seance-09-mur-sous-sol

Ce dossier doit contenir les schémas référencés dans le fichier `seance-09.tex`.

## Images attendues

- **`mur-sous-sol-coupe.png`** — Coupe verticale du mur de sous-sol avec données géotechniques (file C)
- **`mur-sous-sol-diagramme-poussee.png`** — Diagrammes de poussée : terre seule, surcharge seule, et combinaison ELU
- **`mur-sous-sol-diagramme-moments.png`** — Diagramme des moments fléchissants sur les deux travées du mur
- **`mur-sous-sol-ferraillage.png`** — Schéma de ferraillage du mur de sous-sol (sections principales)
- **`poutre-cloison-schema-statique.png`** — Schéma statique de la poutre cloison avec charges concentrées et réactions
- **`poutre-cloison-bielles-tirants.png`** — Modèle de bielles et tirants de la poutre cloison

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

