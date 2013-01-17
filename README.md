Self-Organizing-Maps
====================

This code implements methods for automatic cluster reinforcement and hierarchical cluster visualization of sparsely-matched SOMs , described in: N. Manukyan, M.J. Eppstein, D.M. Rizzo,"Data-driven cluster reinforcement and visualization in sparsely-matched self-organizing maps," Neural Networks and learning Systems, IEEE Transactions on, vol23, no 5, pp 846-852.
ABSTRACT: The Cluster Reinforcement phase advances cluster separation in a self-organizing map (SOM) by strengthening cluster boundaries in a data-driven manner. SOM is a self-organized projection of high dimensional data onto a typically two dimensional (2D) feature map, wherein vector similarity is implicitly translated into topological closeness in the 2D projection. The CR phase amplifies within-cluster similarity in an unsupervised, data-driven manner. Discontinuities in the resulting map correspond to between-cluster distances and are stored in a boundary (B) matrix. CR phase enables a new hierarchical visualization of cluster boundaries displayed directly on feature maps, which requires no further clustering beyond what was implicitly accomplished during self-organization in SOM training. 

The driver function demoCR.m illustrates how to use these functions on an already trained SOM using Kohonen's animal data.

The primary functions are:

CR.m (Cluster Reinforcement Phase for SOM),
B_matrix.m (Create Boundary Distance Matrix),
Plot_B.m (Display B-matrix as a heat map),
PlotBLines.m (Display B-values as grid lines on top of component planes).

Auxilliary functions:
BestMatchingNeurons.m,
BmatrixCbFcn.m,
B_GUI.m,
eucdist.m,
index_of_closest.m.

We also provide SOM code (SOM.m) for users convenience.
