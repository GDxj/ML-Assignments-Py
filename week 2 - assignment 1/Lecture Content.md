1. feature scaling (lessen gradient descent steps, particularly important for polynomial regression)
   - mean normalization (x - mu) / s   s = range or sd
   - standardization
2. Gradient Descent
   - need to choose proper alpha
   - need iteration
   - work well when n (# of features) is large
3. normal equation - analytical solution
   theta = pinv(XT * X) ^ (-1) * XT * y
   - need to compute pinv(XT * X), which is n*n matrix
   - slow if large n
   - not always have analytical solution
   - pinv(XT * X) non-invertable
      * redundent features
