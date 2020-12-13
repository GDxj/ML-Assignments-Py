# Unsupervised Learning
## 1. K means
- iterative
  1. cluster assignment 
  2. move centroid
- input
  1. number of clusters
  2. training set
- random initializtion 
  1. K (number of cluster) < m (number of x)
  2. randomly pick K training data, set initial centroid equal to the data
  3. repeat iteration 50 to 1000 times and pick the one with lowest cost function
- choose number of clusters K
  1. Elbow method
  2. purpose - ex: shirt size, S, M and L
  
## 2. Dimentionality Reduction
- motivation: 
  1. data compression: less memory and speed up learning algorithm
  2. data visualization (normally down to 3D or 2D)
- PCA 
  * goal: minimize projection error
  * steps:
    1. preprocessing (mean normalization/feature scaling)
    2. compute ‘covariance matrix’ Sigma - 1/m * X' * X
    3. compute Eigenvectors - svd
  * Reconstruction
    - x = U * z
  * choosing number of principle components k
    1. average projection error (a)
    2. total variation in the data (b)
    3. choose k so that a/b <= 0.01 --- 99% of the variance is retained
    4. faster way： use S in svd - refer to lecture
  * do not use it to avoid overfitting, use regularization term instead
  
