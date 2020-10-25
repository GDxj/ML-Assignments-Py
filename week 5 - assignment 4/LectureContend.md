# Neural Network Training
- we must account for multiple theta matrices. The number of columns in our current theta matrix is equal to the number of nodes in our current layer (including the bias unit)
- backpropogation
  1. calculate activations using forwardpropogation
  2. calculate error backwards 
  3. calculate partial derivatives of Cost
- parameters unrolling
- gradient checking (numerically estimate derivatives, and compare)
  * turn it off while training model
- random initialization of theta: symetric breaking
  * all 0 does not work

- nn building Steps:
  1. pick network architecture: number of layers, number of units...
     resonable default setting: 1. single hidden year 2. multiple hidden layers with same units (units the more the better but more computaional expensive)
  2. training
    1. randomly initializa weights
    2. implement fp to get h(x) for any x
    3. implement code to compute J(theta)
    4. implement bp to compute partial derivative of J(theta) to each theta
    note: fp and bp, loop over each xi (there are more complex method but not for now)
    5. gradient checking 
    6. optimization to minimize cost function
