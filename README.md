# K-means and K-medoids Clustering Algorithms

This repository contains implementations of K-means and K-medoids clustering algorithms using NumPy and scikit-learn for data preprocessing and visualization.

## Introduction

Clustering is a type of unsupervised learning technique used to group data points into clusters based on their similarities. Here, we implement two popular clustering algorithms:

- **K-means**: Iteratively assigns data points to clusters and updates centroids to minimize the within-cluster sum of squares (WCSS).
- **K-medoids**: Similar to K-means but uses actual data points (medoids) as cluster centers, which are more robust to outliers compared to centroids.

## Dataset Generation

The dataset used for demonstration is generated using `make_blobs` from scikit-learn. It consists of 300 samples, distributed among 4 clusters in a 2-dimensional feature space.

## K-means Clustering

### Steps:
1. **Initialization**: Randomly initialize cluster centroids.
2. **Assign Clusters**: Assign each data point to the closest centroid.
3. **Update Centroids**: Compute the mean of points in each cluster to update centroids.
4. **Convergence**: Repeat steps 2 and 3 until centroids converge or a maximum number of iterations is reached.

### Evaluation:
- **Within-Cluster Sum of Squares (WCSS)**: Measures the compactness of clusters.

## K-medoids Clustering

### Steps:
1. **Initialization**: Randomly initialize medoids (actual data points).
2. **Assign Clusters**: Assign each data point to the closest medoid based on dissimilarities.
3. **Update Medoids**: Select the data point with the minimum sum of dissimilarities within each cluster as the new medoid.
4. **Convergence**: Repeat steps 2 and 3 until medoids converge or a maximum number of iterations is reached.

### Evaluation:
- **WCSS**: Calculated similarly as in K-means, but using medoids instead of centroids.

## Results

Both algorithms are evaluated based on their ability to group data points into meaningful clusters and minimize WCSS. The results are visualized using Matplotlib, showing the original data points and cluster centers (centroids for K-means and medoids for K-medoids).

## Instructions to Run

1. Download or clone the repository.
2. Ensure Python 3.x and required libraries (NumPy, scikit-learn, Matplotlib) are installed.
3. Run the provided script to execute either K-means (`k_means.py`) or K-medoids (`k_medoids.py`) clustering algorithms.

## Conclusion

These algorithms provide efficient ways to cluster data points and identify patterns within datasets. By adjusting parameters such as the number of clusters (k) and the maximum number of iterations, users can tailor the algorithms to suit specific data characteristics and clustering requirements.


![image](https://github.com/idrees200/K-means-and-K-medoids-Clustering-Algorithms/assets/113856749/acc8b898-9a7f-48e9-948e-99821620cf44)
![image](https://github.com/idrees200/K-means-and-K-medoids-Clustering-Algorithms/assets/113856749/e9d80c1f-5f05-4bee-a44e-1de2a1ae5398)
