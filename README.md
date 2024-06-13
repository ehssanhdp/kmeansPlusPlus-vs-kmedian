# KMeans++ and KMedian Clustering Algorithms

This repository contains the implementation and comparison of KMeans++ and KMedian clustering algorithms. The comparison is based on several datasets to evaluate performance in terms of computation time and purity.

## Datasets

The following datasets are used for comparison:

1. **Aggregation Dataset**
2. **D31 Dataset**
3. **R15 Dataset**
4. **Iris Dataset**
5. **Glass Dataset**

## Results

The comparison results between KMeans++ and KMedian clustering algorithms based on the provided datasets are as follows:

### Aggregation Dataset

- **Time**: KMeans++ took less time (1.34 s) compared to KMedian (1.42 s).
- **Purity**: KMeans++ achieved higher purity (0.908) compared to KMedian (0.885).

### D31 Dataset

- **Time**: KMeans++ took more time (22.5 s) compared to KMedian (11.6 s).
- **Purity**: KMeans++ achieved higher purity (0.944) compared to KMedian (0.814).

### R15 Dataset

- **Time**: KMeans++ took less time (1.54 s) compared to KMedian (1.98 s).
- **Purity**: KMeans++ achieved higher purity (0.926) compared to KMedian (0.86).

### Iris Dataset

- **Time**: KMeans++ took less time (44.3 ms) compared to KMedian (47.7 ms).
- **Purity**: KMeans++ achieved slightly higher purity (0.893) compared to KMedian (0.887).

### Glass Dataset

- **Time**: KMeans++ took less time (131 ms) compared to KMedian (220 ms).
- **Purity**: KMeans++ achieved slightly higher purity (0.53) compared to KMedian (0.523).


## Differences 
KMeans++ and KMedian are both clustering algorithms, but they differ in their approach to measuring distance and choosing centroids.KMeans++ uses Euclidean distance to strategically place initial centroids, aiding K-means in minimizing within-cluster variance, selecting initial centroids to improve convergence speed and accuracy. It focuses on minimizing the sum of squared distances between points and their assigned centroids. KMedian, on the other hand, uses Manhattan distance, minimizing the sum of absolute deviations, and calculates centroids based on the median of points within each cluster. This makes KMedian more robust to outliers compared to KMeans++, which is sensitive to extreme values. These differences result in varying performance and clustering purity depending on the dataset.

