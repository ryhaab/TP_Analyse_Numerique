[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ryhaab/TP_Analyse_Numerique/main)
# TP_Analyse_Numerique
 - [Introduction](#Introduction)
- [Generalité](#Generalité)
- [Les méthodes d'integration numérique](#Méthodes_numérique)
  - [Méthode des Rectangles à gauche](#Rectangle_gauche)
  - [Méthode du point milieu](#Point_milieu)
  - [Méthode des trapézes](#Trapézes)
  - [Méthode de simpson](#Simpson)
## Introduction
L'intégration est l'un des problèmes les plus importants rencontrés en analyse. En fait, on rencontre souvent des intégrations, dont le calcul par des méthodes analytiques est très compliqué voire impossible, car il n'y a pas d'expression analytique de la primitive de la fonction à intégrer. Dans ces cas, des méthodes composées peuvent être appliquées pour évaluer la valeur d'une intégrale donnée. La plupart des méthodes d'intégration numérique fonctionnent sur le même principe. Nous divisons d'abord le grand intervalle [a, b] en N intervalles plus petits [ai, ai + 1], où a1 = a et aN + 1 = b. Ensuite, pour chaque intervalle [ai, ai + 1], on essaie d'approximer.
## Generalité
- Si f est une fonction continue sur l'intervalle [a, b], on ne sait généralement pas comment calculer la primitive de f. Par conséquent, si vous souhaitez obtenir la valeur de $$\\int_a^bf(t)\\,dt$$\n, il est parfois nécessaire d'utiliser la méthode intégrale numérique d pour obtenir une valeur approximative. La plupart des méthodes d'intégration numérique fonctionnent sur le même principe. Nous divisons d'abord le grand intervalle [a, b] en N intervalles plus petits [ai, ai + 1], où a1 = a et aN + 1 = b. Ensuite, pour chaque intervalle [ai, ai + 1], on essaie d'approximer. Le moyen le plus simple est :
## Méthodes_numérique
- Décomposition du domaine en morceaux (un intervalle en sous-intervalles contigus)
- Intégration approchée de la fonction sur chaque morceau 
- Sommation des résultats numériques ainsi obtenus.
### Rectangle_gauche
- la méthode des rectangles à gauche : on approche par . Géométriquement, cela signifie qu'on approche l'intégrale de f par l'aire des rectangles hachurés en vert :
### Point_milieu
- la méthode du point milieu : on approche par . Géométriquement, cela signifie qu'on approche l'intégrale de f par l'aire des rectangles hachurés en bleu :
### Trapézes
-La méthode d'intégration approximative introduite par Newton & Cotes, appelée trapèze, est plus précise que la méthode de base appelée rectangle, telle que décrite ci-dessous, et correspond à la somme de Cauchy-Riemann, y compris l'approximation par pas au lieu de la fonction initiale. Graphiquement, dans l'intervalle [xi, xi + 1], nous remplaçons l'arc de la courbe par le segment de ligne [MiNi + 1], de sorte que l'aire sous la courbe est modifiée par rapport au "rectangulaire" xi Mi Ni + 1 xi + 1 (photo de gauche) :
### Simpson
-La méthode de Simpson consiste à regrouper trois points consécutifs des courbes Mi, Mi+1 et Mi+2, et à remplacer l'arc de la courbe passant par ces trois points par un arc parabolique. Veuillez noter que si les points Mi, Mi + 1 et Mi + 2 sont alignés, le calcul du paramètre parabolique de l'équation y = mx2 + px + q, en passant ces points se traduira par m = 0. Dès lors, lorsqu'il s'agit d'une métaphore dégénérée, la situation n'est pas unique.
