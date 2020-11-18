# SVM （large margin classifier)
- make classifier large margin
  * mathametically (see lectures)
- Kernal
  * similarity functions (e.g. Gaussian) - instead of X or Powers of X
- bias - variance
  * large C = small lambda = high bias
  * sigma square large - Guasian kernal fall off relatively slow as change x - high bias low var
- parctice
  * solve theta - recomend using packages
  * choose kernal
    1. no kernal - linear kernal - many features little training data
    2. Gausian kernal - probly the most common kernel
      - **feature scalling** larger feature will dominate when we calculate the Euclidean distance
    3. Mercer's Theorem - faster the optimization by satisfying this tech condition
    4. other kernel (rarely used) - polynomial kernel, esoteric kernels, string kernel, chi-square kernel, histogram intersection kernel
  * choose sigma square
  * multiclass
    1. one vs all
- logistic reg vs svm
  1. # features n > training set size m
    * use logistic reg or svm with linear kernel- not enough data to fit a complex model 
    * n small, m itermediate - svm with linear kernel/Gaussian
    * n << m svm with Gaussian will be slow, instead, manually create more features, use logistic reg or svm without kernel(linear)
    * nn works fine for all senario but sometimes slow to train
- optimization of svm is convex - no need to worry about local optima
- one more note: what matter more than choosing a algorithms is 1. how much data you have 2. how skilled you are 3. error analysis 4. debuging an algorithm (var vs bias)
    
