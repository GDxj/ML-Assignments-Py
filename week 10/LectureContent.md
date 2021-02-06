# Big data
## GD with large datasets
- learning curve to detect if a larger dataset is necessary
- stochastic GD （old one is called Batch GD) （tend to be close enough to global min, not as close as Batch GD）
  1. randomly shuffle/reorder dataset
  2. use each training example a time, modify the parameter a bit and then go to next example (every iteration is on a single example)
  3. repeat step 2 multiple times (1 to 10) depending on training set size
- each gradient step for batch GD: use whole dataset
- each gradient step for stochastic GD: one data point
- mini-batch GD: b example each iteration (b = mini-batch size, typically 2-100), can be faster than stochastic GD by vectorization
