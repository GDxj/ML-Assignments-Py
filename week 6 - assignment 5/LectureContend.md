- When large error in predictions
  1. get more training data
  2. try smaller set of data
  3. try getting additional features
  4. try adding polynomial features
  5. try decreasing lambda
  6. try increasing lambda
- ml diagnositic
  1. what is/isnt working
  2. gain insight of how to improve the model
- training/testing procesure
  1. learn theta using training data
  2. calculate error using test set (test set error or test set cost)
- model selection
  * train/validation/test  60/20/20
  * use validation set to select model
- bias vs variance
- choose lambda
  1. pick lambdas within an interval (0.01, 0.02, 0.04, ..., 10.24)
  2. calculate theta
  3. calculate validation set error
  4. pick lambda with lowest validation error
- learning curve
  * high bias - 1. small gap between Jcv and Jtrain 2. getting more training data does not help much
  * high variance - 1. large gap 2. getting more data likely helps
- **DUMMARY**: debugging a learning algorithm (already applied regularization)
  1. get more traing example - fix high variance (ploting learning curve first to identify high var)
  2. try smaller set of features 
  3. try additional features - fix high bias
  4. getting poly features - fix high bias
  5. decrease lambda - fix high bias
  6. increase lambda - fix high var
