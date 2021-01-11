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
    
