# Étude numérique d'un modèle climatique couplé à l'océan profond

Étude mathématique et numérique de modèles de bilan énergétique (EBM), du modèle global 0-D jusqu'à un modèle zonal couplé à l'océan profond.

Projet de L3 de mathématiques (parcours MApI3, Université de Toulouse, 2025 – 2026), encadré par Judith Vancostenoble, et présenté en soutenance orale.

## Contexte

Les modèles de bilan énergétique décrivent l'évolution de la température terrestre à partir de la différence entre l'énergie solaire reçue et l'énergie infrarouge émise. Malgré leur simplicité, ils font apparaître plusieurs états d'équilibre, dont une Terre entièrement gelée (« Snowball Earth ») et des basculements brutaux entre ces états.

## Contenu de l'étude

**Modèle 0-D** (une seule température moyenne)
- prise en compte de l'effet de serre et d'un albédo dépendant de la température
- existence et unicité des solutions (Cauchy-Lipschitz), trois équilibres (≈ 233 K, 265 K et 288 K) et étude de leur stabilité 
- diagramme de bifurcation en fonction de l'apport solaire : transition vers l'état « Snowball Earth »

**Modèle 1-D** (température dépendant de la latitude)
- transport de chaleur par diffusion, albédo discontinu au niveau de la ligne des glaces

**Modèle couplé à l'océan profond** (Hidalgo & Tello, 2020)
- équation de surface avec diffusion non linéaire (p-laplacien) couplée à une équation de l'océan en profondeur 
- méthode numérique : volumes finis, reconstruction WENO, intégration en temps par Runge-Kutta TVD, condition CFL 
- recherche des équilibres par évolution en temps jusqu'à stabilisation

## Principaux résultats

- Les simulations retrouvent les trois régions prévues par le théorème de Díaz-Tello (une seule solution d'équilibre, puis plusieurs, puis de nouveau une seule) et mettent en évidence jusqu'à **huit équilibres distincts** dans la zone de multiplicité.
- Le couplage avec l'océan profond ne change pas la structure qualitative du problème, mais **réduit fortement l'amplitude des températures** (d'environ 60 °C à 35 °C) ce qui traduit le rôle régulateur de l'océan.

## Fichier

| Fichier | Contenu |
|---|---|
| `Etude-numerique-modele-climat-couplage-ocean-profond.pdf` | Rapport complet avec les démonstrations, les figures et la bibliographie |

## Références principales

- H. Kaper et H. Engler, *Mathematics and Climate*, SIAM, 2013.
- A. Hidalgo et L. Tello, « Numerical Approach of the Equilibrium Solutions of a Global Climate Model », *Mathematics*, 2020.

## Auteur

Badr Chqaf, M1 Data Science, Aix-Marseille Université
