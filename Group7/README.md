Required packages:
- Seurat
- rhdf5
- parallel
- dplyr
- rhdf5
- RANN
- tidyr
- randomForest

Features: We use the following features to build a model.
- "log2_ncell" : log2 of number of cells
- "log2_mean_nUMI": log2 of mean library size
- 'ncell_cluster2': log2 of number of clusters in 2nd cluster
- 'kdist' : distance between 2 centroid produced by k-means in pca space
- 'var_depth_cluster1': variance of depts in cluster1
- 'frequency_cluster2': frequency of cluster2
- 'ncell_big_cluster': number of cells in the big cluster
- 'total.frequency': sum of frequencies of 2 clusters
- 'frequency_big_cluster': frequency of big cluster
- 'total.cells': total number of cells
- 'cluster_balance': #cell in small cluster / #cell in big cluster

Model: We trained the model using random forests.

