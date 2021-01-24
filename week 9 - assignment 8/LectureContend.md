# Anomaly Detection and Recommender Systems
### Anomaly Detection
- p(x) <  epsilon
  1. Fraud detection
  2. Manufacturing (aircraft engines)
  3. Monitoring computers in a data center
- use likelyhood to make decision, assuming Gausian distributed
- evaluation on cv set and test set 
  1. accuracy no good - skewed data
  2. confusion matrix, recall/precision, F1 score
- anomaly detection vs supervised learning
  ad: very small number of positive examples, many different types of anomalies
  sl: large number of pos example, enough pos examples for the algorithm to get a sense of what pos examples are like
- Non-Gaussian features: transformations
- Error analysis, then create new feature to make algorithm cover the error
    
### Recommender System
- ollaborative filtering (can do feature learning by estimating x given theta), also called low rank matrix factorization
  * can iterate: theta -> x -> theta -> x ... (this is doable because the data has multiple people watch multiple movies)
  * but better solution: minimize x and theta simultaneously - no theta0 or x0
    1. initialize x and theta to small random values
    2. minimize J(x,theta) using GD or other optimization
    3. star rating = theta.T * x
- recommend movies: smallest distances between Xs
- mean normalization:  new user who have not rated any movie, all 0s does not make sense
