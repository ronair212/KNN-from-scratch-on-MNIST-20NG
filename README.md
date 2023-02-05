# KNN-from-scratch-on-MNIST-20NG

This code implements a solution to the "MNIST, 20 NG" problem which involves parsing, normalizing features, and computing pairwise similarity matrices. The problem involves working with two different datasets: 20NG (text) and MNIST (images). The solution uses a library/package to parse the datasets.

The 20NG dataset requires text row normalization using either TF (term frequency) or DL (document frequency) and it is important to maintain a sparse format due to the large number of columns. The MNIST dataset is already in a preformatted range [0-255] and may not require normalization, but it is suggested to get the values to have 0 mean instead of 128 mean.

The code normalizes the features using either Shift-and-scale normalization (subtracting the minimum and dividing by the new maximum) or Zero mean, unit variance (subtracting the mean and dividing by the appropriate value to get variance=1).

The code computes the pairwise similarity/distance matrix using a package library available in Matlab/Java/Python/R and includes the following options: cosine or simple dot product, Euclidean distance, editing distance (with a threshold of tolerance on numerical feature values), Jaccard similarity (optional), and Manhattan distance (optional).

KNN - Classification algorithm is implemented from scratch. K-Nearest Neighbor (KNN) is a simple and widely used supervised machine learning algorithm for classification problems. It works by finding the K-nearest data points in the feature space and assigning the class label of the majority of the neighbors to the target data point. The number of nearest neighbors, K, is a hyperparameter that needs to be specified beforehand.

The algorithm stores all the available data points and their class labels. When a new data point is encountered, its distance to each of the stored data points is calculated using a distance metric such as Euclidean distance, Manhattan distance, or Cosine similarity. The K data points with the shortest distances to the new data point are selected as its nearest neighbors. The class label of the majority of the K nearest neighbors is assigned to the new data point as its predicted class label.

KNN has been widely used in many applications, including image classification, pattern recognition, and anomaly detection. It is simple to implement, easy to understand, and has good performance for small datasets. However, it can be computationally expensive for large datasets and may not perform well for highly imbalanced datasets. Classification is performed using a subset of the entire dataset.
