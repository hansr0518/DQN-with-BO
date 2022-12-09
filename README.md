# Bayesian Optimization for DQN
This is a simple experiment of Bayesian optimization for hyper-parameters in Deep-Q-Network.  
To build Deep-Q-Network, we can use simple nueral network with various hyper-parameters.  
Optimizing hyper-parameters is quite time-consuming task and Bayesian-optimization methods will give a quick view of the best combination of hyper-paramters.  
In this experiment, two hyper-parameters (learning-rate, gamma) will be optimized using BO.




## About hyper-parameter
The description of each variable is as follows.  
Note that for Bayesian Optmization, the hyperparameter to be tuned should be passed in a form of tuple.  
| Argument | Description |
|---|---|
|learning-rate| The range of learning rates. (or a value) |
|gamma|Discount factor in DQN|




## About DQN
To find a optimal policy, we can use Q table.  
When states is too large, it is batter to use a neural network.  
The neural network is basically a function approximator for the Q function.  
> * Input : State  
> * Output : The Q-values for each action in the action space.  
> * State space: 4 continuous values  
>   1. cart position
>   2. cart velocity
>   3. pole angle
>   4. pole velocity at the tip
> * Action space: 2 discrete actions
>   1. push cart to the right
>   2. push cart to the left
> * Reward : acquires +1 reward for every timestep until the termination  
>           (Well builted DQN model has a return value more than 200) 




## result
> The initial value 
> * gamma : 0.98 
> * learning rate : 0.0005


> The result of Bayesian-optimization 
> * gamma : 0.82
> * learning_rate: 0.000691
