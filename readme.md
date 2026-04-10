📊 Rapport Final de Projet Data Analyst : Maîtrise Statistique
Ce rapport présente les résultats d'un sprint d'analyse de données axé sur la maîtrise des concepts statistiques fondamentaux et leur application pratique sur deux datasets réels : la santé publique et l'automobile.

🛠️ Phase 1 – Fondamentaux Statistique : Compréhension & Documentation
Cette phase pose les bases théoriques nécessaires à toute analyse de données fiable. Une documentation complète de chaque notion a été produite.
📚 Concepts Clés Abordés :
* Statistiques descriptives : Moyenne, médiane, variance, écart-type, histogramme, boxplot.
*Population vs Échantillon : Définitions, méthodes d'échantillonnage et leur justification.
*Probabilités et distributions : Bernoulli, Binomiale, Poisson, Normale (Gaussienne), Student, Chi-deux.Théorème Central Limite (TCL) : Principe d'approximation d'une moyenne d'échantillons par une loi normale.
*Échantillonnage et estimation : Évaluation des biais, intervalles de confiance.
*Tests d'hypothèses : Formalisation (H0/H1), p-value, interprétation et prise de décision avec risque $\alpha$.

Phase 2 – Application Pratique 1 : Analyse de Santé Publique
Dataset : healthexp.csv (Données mondiales sur les dépenses de santé et l'espérance de vie).
📈 Visualisations Clés et Résultats
Nous avons réalisé plusieurs visualisations pour analyser l'évolution des dépenses et de l'espérance de vie, ainsi que la relation entre ces deux variables. L'image suivante compile les graphiques clés générés pour cette phase (et pour la phase suivante sur l'automobile).

Figure 1 : Compilation des visualisations clés des deux phases du projet.

🔍 Analyse Approfondie :

1. Nature des Variables
*Variables Continues : Spending_USD, Life_Expectancy.
*Variables Discrètes / Catégorielles : Year, Country.2. Focus sur Spending_USD

2. Analyse univariée :
*L'histogramme et le boxplot des dépenses montrent une forte asymétrie.
*Définition précise de la moyenne : La moyenne de Spending_USD représente la dépense de santé moyenne par habitant, calculée pour l'ensemble des observations du dataset (tous pays et toutes années confondus). Elle est fortement influencée par les valeurs très élevées des USA.

3. Évolution Temporelle
*Durée de vie : On observe une tendance générale à la hausse dans tous les pays, avec une stagnation apparente ces dernières années aux USA.

*Amélioration du graphique : Un graphique en lignes (lineplot) utilisant une couleur différente pour chaque pays est bien plus lisible qu'un scatterplot unique pour cette analyse.

*Dépenses Allemagne vs Grande Bretagne : Le graphique 2x2 (Haut, Centre-Droit) montre que l'Allemagne a des dépenses de santé nettement plus élevées que la Grande Bretagne sur toute la période, bien que la trajectoire soit similaire.

4. Relations et Anomalies
*Relation (USA, 2000-2020) : On note une relation positive : l'espérance de vie augmente avec les dépenses, mais la pente de cette augmentation semble faiblir malgré la hausse massive des coûts.

*Valeur Aberrante (Outlier) : Les États-Unis sont l'aberration majeure. Ils dépensent considérablement plus que tout autre pays, pour une espérance de vie qui est souvent inférieure à celle de pays plus économes. C'est l'un des "bruits" visibles sur le graphique d'évolution des dépenses.

5. Analyses Statistiques AvancéesCorrélation (SpendingUSD / LifeExpectancy) : 
*La corrélation de Pearson pour les USA sur 2000-2020 est extrêmement forte (proche de 0.9+). La p-value associée est quasi nulle, indiquant que cette relation n'est pas due au hasard (H0 rejetée).
*Test d'hypothèse (Bonus) : Pour l'affirmation du politicien (+0.3 an/an aux USA depuis 1970), le test d'hypothèse (avec un niveau de confiance de 98%, $\alpha = 0.02$) a été réalisé. Les résultats précis des tests peuvent être trouvés dans le code d'analyse joint.

🚗 Phase 3 – Application Pratique 2 : Dataset Automobile MPG
Dataset : MPG (Données sur la consommation et les caractéristiques des voitures, 1970-1982).

📈 Visualisations Clés et Résultats
Cette phase a utilisé les graphiques visibles en bas et à droite de la compilation de la Figure 1 pour analyser les tendances de consommation automobile.

🔍 Analyse Approfondie :
1. Nature des Variables
*Variables Continues : mpg, horsepower, weight, acceleration.

*Variables Discrètes / Catégorielles : cylinders, model_year, origin.

2. Analyse de mpg (Consommation)
*Définition précise de la moyenne : La moyenne de mpg (Miles Per Gallon) représente l'efficacité énergétique moyenne de l'ensemble des modèles de voitures testés dans le dataset entre 1970 et 1982. Plus elle est élevée, moins la voiture consomme de carburant.

*Visualisation univariée : L'histogramme et le boxplot (Figure 1, Bas-Gauche et Bas-Centre) montrent une distribution étalée avec quelques modèles très sobres (haut MPG), mais une majorité située entre 15 et 30 MPG.

3. Relations Clés
*mpg vs horsepower : Il y a une corrélation négative forte. Plus la puissance (horsepower) augmente, plus la consommation de carburant est élevée (MPG baisse).

*Ajout de model_year : En analysant par année, on observe une tendance : les modèles plus récents tendent à avoir un meilleur MPG pour une même puissance par rapport aux modèles plus anciens. L'efficacité s'améliore.

*Poids moyen des voitures US (70-82) : On voit une tendance claire à la diminution du poids moyen des voitures américaines, en particulier à partir de la fin des années 70.
!<[alt text](image.png)




*cylinders vs model_year : Le scatterplot (Figure 1, Droite) illustre une transition historique. En 1970, on voit beaucoup de moteurs 8 cylindres (les points du haut). Avec le temps, ces points disparaissent, au profit des 4 cylindres (les points du bas). C'est le "downsizing".

"# simplone"  
"# simplone"  
