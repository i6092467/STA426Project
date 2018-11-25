# Comparison of Dimensionality Reduction Techniques for RNA-seq Data - STA 426 Project

This project is intended for STA 426 course and will be written by Ricards Marcinkevics (GitHub username: i6092467).

In this project we would like to compare different dimensionality reduction techniques (PCA, MDS under various distances, t-SNE, LLE etc.) w.r.t. their ability to preserve treatment effect signals. 
* We will choose 2-3 *source* RNA-seq raw count datasets and, possibly, normalise them to remove unwanted variation. We could also perform the comparison in presence of the unwanted variation.
* We will simulate datasets from the *sources* using a non-parametric [SimSeq][1] approach. Datasets will be simulated under two settings: the global null and differential expression.
* We will compare dimensionality reduction methods by measuring how well treatment clusters are separated in the reduced space. Possible criteria for comparison include average silhouette width (ASW), within-cluster sum of squares, within-class and between-class variance ratio, accuracy of the nearest neighbour algoritm (1-NN) when predicting treatment group in the reduced space etc. Note, that herein samples will be assigned to clusters according to their treament group.
* We will aggregate the performance measures across simulated datasets for different sources for each method to draw final conclusions.

[1]: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4481850/ "SimSeq: a nonparametric approach to simulation of RNA-sequence datasets"
