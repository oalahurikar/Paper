## Why use Unscented Kalman Filter:
The UKF does not need to linearize non-linear functions; instead, the UKF takes representative points (Sigma Points) from a Gaussian distribution. These points will be plugged into the non-linear equations in order to make estimate.
The nonlinearity can occur in the process model because of bearing dynamic friction, rotational elements and phenomena such as misalignment, imbalance, and overturning moment.
It can be difficult to transform whole state distribution through nonlinear function as shown in figure 1 but it’s easy to transform individual points of state space through nonlinear function as shown in figure 2. Sigma points are chosen at mean state and standard deviation of every state dimension. 

| header 1 | header 2 |
| -------- | -------- |
| ![alt_text-1](https://github.com/oalahurikar/Paper/blob/master/Images/Sig%20Pts%20Trans.png) | ![alt_text-2](https://github.com/oalahurikar/Paper/blob/master/Images/Sig%20Pts%20dis.png)   |


