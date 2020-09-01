1. feature scaling (lessen gradient descent steps, particularly important for polynomial regression)
   - mean normalization (x - mu) / s   s = range or sd
   - standardization
2. Gradient Descent
   - need to choose proper alpha
   - need iteration
   - work well when n (# of features) is large
3. normal equation - analytical solution
   theta = (XT * X) ^ (-1) * XT * y
   - need to compute (XT * X) ^ (-1), which is n*n matrix
   - slow if large n
   - not always have analytical solution
   - pinv(XT * X) non-invertable (singular)
      * redundent features (colinearity) : delete one of them
      * too many features (m << n) : delete some features, or use regularization
