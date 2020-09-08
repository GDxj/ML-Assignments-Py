## Logistic Regression

1. Cost Function
  -identical to linear regression; h_theta changed (sigmoid transformation)
  
2. Other opnimazation algorithems (other thank GD)
  - Conjugate Descent
  - BFGS
  - L-BFGS
    * pick alpha automatically at each iteration; converge much faster than GD
    * Adv and Disadv:
      1. no need to pick alpha
      2. faster than GD
      3. more complex
    
 3. Multiclass classification (i class)
   - one vs all: build i classfiers (similar to idea of dummy variable)
   - pick i that max(h(i)) where h(i) is the ith classifier and h(i) means the probabily of being that specific class
   
 4. Regularization
   - Underfittin = high bias
   - Overfitting = High variance : too many features, do well on training set but not test set/prediction
     * solutions:
       1. reduce number of features
          - manually select features
          - model selection
       2. regularization
          - keep all features, but reduce magnitute/value of parameter theta (when we have a lot of slightly useful features, each contribute a bit to prediction new examples)
          - add penalty (regularization) term to cost function; lambda is called regularization parameter
            * lambda: train the model well and keep # of parameters small
          - not penalize theta0
          - make normal equation always invertable
