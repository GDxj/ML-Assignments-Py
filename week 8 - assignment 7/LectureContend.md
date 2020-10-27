# Unsupervised Learning
## K means
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
