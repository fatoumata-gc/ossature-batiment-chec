# Images de la séance : seances-05-06-poutre

Ce dossier doit contenir les schémas référencés dans le fichier `seances-05-06.tex`.

## Images attendues

- **`poutre-etudiee-vue-plan.png`** — Vue en plan de la poutre étudiée (file~B, travée 1-2) et schéma des charges supportées
- **`poutre-schema-charges.png`** — Schéma statique global de la poutre continue avec charges concentrées $G$, $Q$ et charges réparties $g$, $q$
- **`poutre-courbe-enveloppe.png`** — Courbe enveloppe des moments fléchissants sur les deux travées B1-B2 et B2-B3
- **`poutre-epure-arret-barres.png`** — Épure d'arrêt des barres --- courbes enveloppes décalées de $a_l = 0{,}28$~m et schéma de ferraillage en élévation
- **`poutre-coupe-section.png`** — Coupes de la section en appui B1, en travée et en appui B2 avec disposition des armatures longitudinales et des cadres
- **`poutre-suspentes.png`** — Schéma des armatures de suspente au droit de l'appui de la poutrelle sur la poutre principale

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

