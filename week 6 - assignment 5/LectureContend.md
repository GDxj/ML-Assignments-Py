# Model Debugging
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
- **SUMMARY**: debugging a learning algorithm (already applied regularization)
  1. get more traing example - fix high variance (ploting learning curve first to identify high var)
  2. try smaller set of features 
  3. try additional features - fix high bias
  4. getting poly features - fix high bias
  5. decrease lambda - fix high bias
  6. increase lambda - fix high var
- （after ex5) machine learning system design: example - spam classifier
  1. collect lots of data - e.g **honeypot project**
  2. develop more sophisticated features on the email （from email header)
  3. develop more sophisticated for msg body
  4. develop sophisticated algorithm to detect mispelling
- Error Analysis
  1. start with a simple model
  2. plot learning curve to diagnoze the model
  3. manually examine the examples in validation set that the model made mistake on, and see if there is any systmatic trend/what type of example it is making mistakes on
  4. numberical evaluation is important (validation error)
- Error metrics for skewed classes
  * precision/recall: if predict all 0, we will have 0 recall
  * Trading Off Precision and Recall
    F score = 2*P*R/(P+R)    on validation set
- useing large data sets
  * massive features + large data sets = perfect
  
    
