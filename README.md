# Salmon Contamination Analysis
A comprehensive analysis of contamination levels in farmed salmon from around the world. 

The analysis explores the levels on 9 different contaminants and aims to inform both consumers and businesses on regions which produce salmon with the least contaminants. This information is crucial to businesses and consumers as contamination levels in produce such as salmon vary in different regions relating to a regions historic use of different pesticides. 

The information in this analysis should provide insight into the best regions to source salmon from to reduce the harmful health effects of pesticides in produce. 

## Overview
The objective of this research is to identify the different degrees of contamination present in salmon from differen farmed globally. 

## Dataset

The “farmedSalmon.csv” data file contains the contamination profiles of 153 salmon from 8 different salmon farms located in Europe, North America and South America.The levels of nine contaminants Mirex, Hexachlorobenzene, HCH gamma, Heptachlor Epoxide, Dieldrin, Endrin, Chlordane, DDT and Dioxin are examined. The salmon samples originate from 8 salmon farms around the world.

## Analysis 

The data was first analysed to check for any grouping in the data through the use of cluster analysis. The optimal number of clusters was first tested by plotting the "Total within sum of squares" (Total WSS)  against the cluster number as shown below. The Total WSS refers to the sum of  squared differences between each point in a dataset and the mean of it's respective group. As the plot shows a steep descent until 3 clusters is reached it can be assumed that 3 clusters best fits the data. 

![plot of optimal cluster number](salmonImages/optimalCluster.png)


The cluster number was then checked by plotting cluster plots showing between 2 and 4 clusters to fit the data. The cluster plots confirmed that the optimal cluster number is three. The two cluster plot doesn't achieve much separation between the two groups in the data. The four cluster shows over fitting with the two clusters in the middle of the plot having significant overlap.


![grid of cluster plots](salmonImages/clusterGrid.png)


The locations of the salmon farmed are then plotted on a world map to identify groups of salmon farms which are geographically close. As shown in the cluster analysis there were 3 distinct groups identified through spatial analysis, being the continents Europe, North America and South America.  



![salmon farm locations world map](salmonImages/worldmapPlot.png)














Principle Component Analysis (PCA) is first applied to identify any trends between different salmon sources. A country based PCA shows significant overlap between countries of the same continent indicating a continent based PCA may be more suitable. 








A continent based PCA shows much better group separation therefore the following analysis is conducted comparing the contamination levels in different continents.





![continent based PCA plot](salmonImages/continentPCAplot.jpg)

Density plots are used to examine the contamination levels present in the different continents. 

![grid of contaminant density plots](salmonImages/densityGrid.png)









## Tools Used 
* **R Studio**: Data prep and cleaning, Principal Component Analysis, Cluster Analysis, Linear Discriminant Analysis and visualisation. 

## Conclusions 

## Acknowledgements
