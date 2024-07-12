# Clustering Methods in Python


## 1. K-Means Clustering

**K-Means** clustering aims to partition the data into `k` clusters, where each data point belongs to the cluster with the nearest mean. It is a centroid-based algorithm that iteratively updates cluster centers to minimize the variance within each cluster.

### Key Points:
- Requires the number of clusters `k` to be specified.
- Sensitive to initial placement of centroids.
- Can converge to local minima.

## 2. Hierarchical Clustering

**Hierarchical Clustering** builds a hierarchy of clusters either agglomeratively (bottom-up) or divisively (top-down). Agglomerative clustering starts with each data point as its own cluster and merges the closest pairs until only one cluster remains.

### Key Points:
- Does not require the number of clusters to be specified initially.
- Can produce a dendrogram, which is a tree-like diagram of clusters.
- Computationally intensive for large datasets.

## 3. DBSCAN (Density-Based Spatial Clustering of Applications with Noise)

**DBSCAN** is a density-based clustering algorithm that can find arbitrarily shaped clusters and identify outliers. It groups together points that are closely packed together and marks points that are far away as outliers.

### Key Points:
- Does not require the number of clusters to be specified.
- Requires two parameters: `eps` (maximum distance between points in a cluster) and `min_samples` (minimum number of points in a cluster).
- Can handle noise and outliers effectively.

## 4. Mean Shift Clustering

**Mean Shift** is a centroid-based algorithm that updates candidates for centroids to be the mean of the points within a given region. It does not require specifying the number of clusters in advance and can find the number of clusters automatically.

### Key Points:
- Automatically determines the number of clusters.
- Computationally intensive for large datasets.
- Sensitive to the bandwidth parameter.

## 5. Gaussian Mixture Model (GMM)

**Gaussian Mixture Model** (GMM) is a probabilistic model that assumes all the data points are generated from a mixture of several Gaussian distributions with unknown parameters. It uses the Expectation-Maximization (EM) algorithm to estimate the parameters.

### Key Points:
- Can handle clusters of different shapes and sizes.
- Provides a probabilistic clustering.
- Requires the number of clusters `k` to be specified.

