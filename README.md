# Bayesian Optimization for DQN
This is a simple experiment of Bayesian optimization for hyper-parameters in Deep-Q-Network.  
To build Deep-Q-Network, we can use simple nueral network with various hyper-parameters.  
Optimizing hyper-parameters is quite time-consuming task and Bayesian-optimization methods will give a quick view of the best combination of hyper-paramters.  
In this experiment, two hyper-parameters (learning-rate, gamma) will be optimized using BO.

--------------

The description of each variable is as follows.
Note that for Bayesian Optmization, the hyperparameter to be tuned should be passed in a form of tuple.
| Argument | Description |
|---|---|
|learning-rate| The range of learning rates. (or a value) |
|gamma|Discount factor in DQN|
