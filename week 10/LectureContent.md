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
- stochastic GD convergence
  1. compute cost before updating theta using xi, yi
  2. every 1000 iterations (say) plot cost averaged over the last 1000 examples processed by algorithm
- can slowly decrease alpha (typically constant)
## online learning (have a continous stream of data coming in)， similar to stochastic GD but just learn from new data
- can adapt changing user preference
- no need to process more than once
## map-reduce and data parallelism  
- split training set into multiple machines
- before applying, make sure the algorithem can be expressed as a summation over the training set
